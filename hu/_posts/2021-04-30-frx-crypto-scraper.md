---
layout: post
title: Crypto FRX árfolyam begyűjtő
lang: hu
lang-ref: frx-crypto-scraper
tags:  [microservice, kubernetes, crypto, scraping]
---

A crypto valuták árfolyama sokakat érdekel, bár sajnos egyelőre nem
váltották be a forradalmi igéreteiket - noha a techológia forradalmi.

Az alkalmazás több microservice összecsomagolásából született, ahol 
időzítve futó script begyújti az árfolyamot és Kafka topicba küldi tova.
Innen pedig adatbázisba kerül, amit Grafana diagrammon látni is lehet.
Az egészet egy helm chartba foglalva lehetséges telepíteni.

![frx-crypto-scrape-demo-ms](/artifacts/frx-crypto-diagram.png)


<!-- more -->
[frx-crypto-scrape-demo-ms a github-on](https://github.com/lsmhun/frx-crypto-scrape-demo-ms)

## Képernyőképek
![ETH and BTC charts](/artifacts/frx-crypto-demo-01.png)