---
layout: post
title: "Sacramento Parking, Open Source Style"
date: 2015-12-20
categories: 
published: true
---

#### **Updated 2015-12-20**

### Story

Back when I first moved to Sacramento, the first challenge I faced was where to park for work.. the wait list at my building is about 10 years, and paying $150+ a month to park for 20 days a month didn't appeal to me. For a time I was fortunate to find a local business that allowed me to park daily for a reasonable rate. 

As I became involved with Code for Sacramento and Open Data, I was pleasantly surprised to find out the City of Sacramento publishes a Open Data set on every single parking space in the downtown area, on their open data portal [http://data.cityofsacramento.org/](http://data.cityofsacramento.org/). It contains information down to the exact geo-coordinated latitude and longitude, along with other associated data. I figured it was worth a shot to find free parking.. and find it I did. 

Because of the format of the data from the Junar open data portal platform, it required parsing to "flatten" out and knowing nothing about python at the time, I fumbled around with a parser written by fellow Code for Sacramento team member Jay Venti. Eventually getting it to work so I could filter down to "all day unrestricted parking" spots was easy, but visualizing it became the challenge.

Fast forward a month, or six.. my interactions with geo genius Kari Mah led me to cartodb, the free to use mapping solution for the geo-dev challenged like myself. After a simple delimited upload, I had a pretty map of Sacramento littered with a grid of dots. Filtering down gave me the gold I was panning for, ALL DAY FREE PARKING SPOTS! Of course with publicly released data (or any data) there is the potential of validation issues, so I took a bike ride to check out the findings. True to form many of the spots were no longer zoned as such, but surprisingly many/most of them were, including some onesy twosy spaces in places nobody would ever think of.

A link to the interactive map is here for all you Sacramento-ans to check out; there are potentially many other uses of this data, including examining zoning effectiveness and the impact of parking on traffic (heuristic, unless you can link it to another data set). I was also able to use the discrete permit area feature of the data to see where permit areas were delineated (picture below).

If anybody has time and would like to fancify this into a more user friendly interface to present to the world, let me know I would love to work with a geo dev on something like a leaflet open street map deploy. 

[Click here for the parking map](https://crosskonaftw.cartodb.com/viz/6adf39d0-fd09-11e4-a589-0e9d821ea90d/public_map)

[Click here for the permit area map](https://crosskonaftw.cartodb.com/viz/ee4d102c-ff1a-11e4-96a4-0e0c41326911/public_map)

*Article still under dev, incomplete.. enjoy whats here in the moment!

![permit areas](/assets/permit_areas.png)
