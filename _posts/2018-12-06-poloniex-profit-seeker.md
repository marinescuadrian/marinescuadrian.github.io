---
layout: post
title:  Make Profit on Poloniex.com exchange
date:   2018-12-06 12:00:00
categories: Cryptocurrency Exchange Blockchain Personal
tags: Cryptocurrency Exchange Blockchain Personal Script Tool
---

It's been a long time since I wrote an article here and today I would like to explain a strategy on how to make some profit on a single exchange by leveraging on different pairs. 

**DISCLAIMER: I haven't tested this method yet, it's still in a theoretical stage and I don't advise anyone to use this method with money that can't afford to lose.**

First of all, we all know that there are small gaps between pairs of a currency on BTC and FIAT (USDT, USDC, etc), even much more when we are talking about total different markets (Poloniex.com, Binance.com, Bittrex.com, etc). 

Let's take a simple case: BTC/ETH is valued at 85$ (FIAT), USDT/ETH is valued at 86.5$ (FIAT), USDC/ETH is valued at 87$ (FIAT). We also know that USDT and USDC are stable coins that should be pegged 1:1 rate to the USD (*cough* not today *cough*). Anyway, there's also a gap between USDT and USDC that can also be exploited for some profit.

I wrote a simple script to do all the maths in real-time using Websockets connected to the Poloniex's order book in order to provide us with accurate data. 

**You can check the script at [https://adrian.marinescu.ch/poloniex-profit/](https://adrian.marinescu.ch/poloniex-profit/)**

What are your thoughts about this? Write your comment below!