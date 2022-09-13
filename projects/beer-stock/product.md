---
order: 100
icon: light-bulb
---

# Product Design

It all started when a friend of mine (the bar owner) said to me that a lot of beer casks are being thrown away due to their expiration dates.
These beers, were not bad, actually, some of them tasted really good (at least to my perception). However, people had the lack of interest in tasting new kind of beer.

!!! :question: How do we make people buy beers that they have never tasted before? :question:
That's easy, one can simply give a discount / lower the price.

Managing such discounts on various types of beers requires analysis of sales closely, but this is a tedious task without analyst tools.

There is another problem with price modification: a customer that visits the local bar several times a month doesn't feel comfortable when the price change on daily basis / weekly basis. 
Customers tend to memorize the price of what they bought, thus, we wouldn't want to raise the price of a specific product and make some returning customer upset.

There is a third problem with this price modeling: how can you maintain the local bar's income for a single night giving such discounts?
!!!


!!! :bulb: How do we make customer try new beers, without analyst tools, without making a returning customer upset affecting the price of his favorite beer for a full night? :bulb:
This thinking is what lead to the creation of Beer Stock.
If we change the price (up or down) of a beer several times througout the night (pracically based on a 7-minute ticker), we could achieve our goals without making a single customer upset for not buying his favorite beer in the price he is used to
!!!

Beer stock price modeling example:

Imagine that this was the end-of-day sales chart before the beer stock:

| Beer Type | Average Beer Price | Count Sold | In Stock |
|-----------|--------------------|------------|----------|
| A         | 25                 | 100        | 0        |
| B         | 28                 | 10         | 90       |
| C         | 27                 | 10         | 90       |


The total income would be: $25 \cdot 100 + 28 \cdot 10 + 27 \cdot 10 = 3,050$

If this would be the status for several days, B and C casks would get thrown away.


With beer stock:

| Beer Type | Average Beer Price | Count Sold | In Stock |
|-----------|--------------------|------------|----------|
| A         | 26                 | 50         | 50        |
| B         | 26                 | 35         | 65       |
| C         | 26                 | 35         | 65       |


The total income would be: $26 \cdot 120 = 3,120)$

This implies a higher income while avoiding throwing away beers B & C!