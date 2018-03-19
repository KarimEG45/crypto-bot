# crypto-bot

[![Join the chat at https://gitter.im/trading-bot/Lobby](https://badges.gitter.im/trading-bot/Lobby.svg)](https://gitter.im/trading-bot/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

<a href="https://travis-ci.org/jnidzwetzki/crypto-bot">
  <img alt="Build Status" src="https://travis-ci.org/jnidzwetzki/crypto-bot.svg?branch=master">
</a><a href="https://scan.coverity.com/projects/jnidzwetzki-crypto-bot">
  <img alt="Coverity Scan Build Status"
       src="https://scan.coverity.com/projects/15223/badge.svg"/>
</a><a href="http://makeapullrequest.com">
 <img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg" />
</a>

This repository contains a crypto currency trading bot. The bot implements some strategies (donchian, ema, atr) and works on the Bitfinex crypto currency exchange. In addition, the project contains some backtesting tools.

**Warning:** Trading carries significant financial risk; you could lose a lot of money. If you are planning to use this software to trade, you should perform many tests and simulations first. This software is provided 'as is' and released under the _Apache 2.0 license_. 

## Installation

Clone the repository and add at least one API key to the `auth.properties` file. The bot is able to trade multiple Bitfinex accounts in parallel. 

Configuration example for one account:

```
apiConnections=1
apiKey.0=<YOUR-API-KEY>
apiSecret.0=<YOUR-API-SECRET>
```

Configuration example for two accounts:

```
apiConnections=2
apiKey.0=<YOUR-FIRST-API-KEY>
apiSecret.0=<YOUR-FIRST-API-SECRET>
apiKey.1=<YOUR-SECOND-API-KEY>
apiSecret.1=<YOUR-SECOND-API-SECRET>
```

After the configuration is done, you can start the `EMABot` or the `DonchianBot`.

## What's next?
* If you like the project, please star it on GitHub!
* If you are interested in the Bitfinex API implementation, see my other project at [https://github.com/jnidzwetzki/bitfinex-v2-wss-api-java](https://github.com/jnidzwetzki/bitfinex-v2-wss-api-java)
