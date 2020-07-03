---
layout: post
title: "Making sense of COVID data."
date: 2020-07-02
excerpt: "Making sense of COVID-19 numbers locally, nationally is important when most media just keeps repeating them without much explanation."
bigimg: /img/covid/summary.png
tags: [COVID19, Corona Virus, India]
comments: true
published: true
---

Making sense of COVID-19 numbers locally, nationally is important when most media sources just keeps scaring everyone using the total numbers as a score. It is important to understand the context & process behind each and what that number really means. I hope this post sheds some light on the same.

## Numbers at High level

We need to understand total number of cases includes Active, Recovered and Deceased. Yes read that again, total number also includes Recovered and Deceased. So every day when we say today there are X cases, we actually need to check how many are Active cases.

ex: If on any day 1000 are new cases, 400 get recovered on same day, 10 were deceased, then on that day the active cases increased by 1000 - 400  - 10 = 590.

This number matters as it truly reflects what is the stress being put on the healthcare systems in your area.

### Who Reports the numbers?

This is an exercise in coordination between with all approved labs, Taluka administrations, Nagar Palikas, State govts, ICMR and center.

You should by now know who reports the numbers for your locality and how to access them. Some bodies put it up online, some draft daily reports. Your local number matters more than state or Country, as that would give you a true picture of how much precautions you need to take and where.

### Which tests are possible?

Source: [ICMR Tests](https://www.icmr.gov.in/cteststrat.html)

#### Molecular based Test (RT PCR/TruNat/CBNAAT)
The test is done for all right now, it detects virus in our throat via a throat swab. Time for report usually under 24hrs.

#### Rapid Antigen Detection Test
This is a newer test, however as per reports the accuracy is less. Time for report usually under 30mins.

#### Antibody testing
Antibody test not only detect if you are positive but also check if you recovered on your own without any medication. Such tests are being carried out at random (no cost) among the population in many hotspot cities across the world, including by India. This is mainly to find out true picture of how widespread the impact of infection is and what is the real mortality rate.

Source: [Reports of First such antibody test in India](https://www.newindianexpress.com/nation/2020/jun/08/15-30-people-in-containment-areas-exposed-to-covid-19-icmrs-serosurvey-2153893.html)

## Testing Strategy

Some people say why can’t we test everyone, that is a foolish argument, you can’t test all population even if you want to. Given the incubation period of 14 days, 100% coverage is very difficult. So this route is a waste of already scarce resources.

Then how to decide whom to test? This is done by a strategy as below,

   1. Test all **symptomatic patients & their family** (high fever, sore throat, etc, or any other COVID19 symptoms)
   2. Test all high risk contacts of **#1** even if asymptomatic. Lets call the 1st and 2nd group of people as **High Risk Individuals or HRI**
   3. Inform contacts of HRI via contact tracing to self quarantine.

Above **#1**, **#2** and **#3** are to be followed strictly but this is where issues start to happen. Ensuring **#2** and **#3** is where everything goes wrong, if local administration is not strictly following protocol.

For example, in Maharashtra asymptomatic are not tested now, which is a huge gap.
Source: [Maharashtra not testing asymptomatic](https://www.timesnownews.com/india/article/maharashtra-not-testing-asymptomatic-cases-hiding-real-picture-of-covid-19-crisis-devendra-fadnavis/583229)

In another contradictory news item the [CM reported that 80% of MH cases are asymptomatic](https://www.news18.com/news/india/80-covid-19-patients-in-maharashtra-asymptomatic-says-uddhav-thackeray-amid-concerns-of-silent-spread-2593463.html) which means it is even more important to test them as they unknowingly might be carriers for other people.

## Growth Rate (lower is better)

This is India's infection growth rate as of 2nd July 2020.

![Growth Rate](/img/covid/growth-rate.png)

Growth rate simply put is how much days it takes for your "active" cases to double. A higher doubling rate means new patients have to be admitted before earlier patients are getting better hence increasing pressure on healthcare system. Our national doubling rate as per above is 25-30 days which is good.

## Why lockdowns?

Healthcare systems are built on a ~5% basis, you assume at any point in time only 5% of the people will need serious healthcare support. In India this number is highly skewed. Far less hospitals in rural, T3, T4 towns and far more in T1 and T2 cities. Rural facilities are often old, less staff, less stock of supplies vs urban facilities have easy access to stock, staff is more and better qualified. As you develop, the the 5% number keeps getting better.

You cant correct 50-60 yrs worth of Healthcare backlog in weeks, you cant ask invisible infection to stop. So what do you do? Lockdown!

The intention was to gear up, take a stock of supplies, set up tracking, coordination with various bodies, prioritize the resources, etc. Lockdown also meant the virus had less persons to infect hence the growth rate was brought down to a level that was manageable by the healthcare system. All states were asked to setup temporary hospitals and beds based on certain projections as per population density, etc.

Check the below projection of what the numbers would have been had there been no lockdown.

**If 7 day doubling it would have been ~3589% higher 2,16,03,269 total cases.**

![Total](/img/covid/total.png)

## Positivity Rate (lower is better)

The most important is positivity rate. This is simply how many tests you do in a day and how many of those are positive. Some also count it as positive per 100 tests. This basically means if the number is low it is a good sign that you are testing all HRI and in control. If this number is high, it means you need to do more tests and much job at tracing HRI so they are quarantined before they infect others.

Maharashtra did 25k tests on 1st July, out of which 5k were positive, which means 1 in 5 tests is positive, which is a 20% positivity rate. In Delhi, before the centre took over and increased testing, on 15th June (15 days ago), Delhi did 6k tests and 1.6k positive, so a positivity rate of 26% even worse than Maharashtra. Compare this with 1st July, when Delhi did 20K tests out of which 2.2k are positive, so the rate falls to 11% still higher than national average of 8% but better than it was 15 days ago.

Hence everything goes back to are you testing all people that are high risk and need testing or are you leaving them to be tested later hoping some dont get infected?.

Check the below image which is a 7 day moving average, you can clearly see which states the curve is dipping (means positivity rate falling), stable or increasing. If it is increasing, testing needs to be increased for HRI.

![Confirmed](/img/covid/confirmed-rate.png)


## Recovery across states (higher is better)

All India recovery are now more than active.

### Recovered (59.4%) + active (37.6%) + deaths (3%)

![recoveries](/img/covid/recovery.png)

Most states more or less have breached the 50% barrier (Recovery is more than Active) or are hovering around it. Which is great news, but it is hardly time to celebrate until there is a considerable gap between two.

## Fatality rate (lower is better)

Death rate or Fatality rate means, for how many people out of the confirmed cases the disease is fatal.

**Fatality rate = Confirmed cases / Deceased * 100**

![Global death rate](/img/covid/worldd.png)

![India death rate](/img/covid/Indiad.png)

Both the above graphs show a different picture, when averaged, India's death rate is very good compared to many western developed nations. The only countries doing better than India are South Korea and Japan. For China, data not released since March so this is a old number and highly unreliable.

When we compare this to our state level data, We can see that four states are above national average. 2 are significantly higher, Delhi is 11x bad of national average and Maharastra is 5x bad.

## Precautions

Various studies both national, international have shown that the best defense which is cheap and easy is to wash hands and wear masks. Personal hygiene and sanitization play a huge role in this disease.

Follow all guidelines as given by the authorities religiously.

Some common sense precautions we take at our home,

1. Wash all veggies properly once brought from outside, if possible soak in salt water for few hours before use or store.
2. Mask and sanitizer bottle is must when going out.
3. No touching of any body or face area when outside.
4. Use sanitizer every time you interact with any object outside (car door, currency, lift buttons, store counter, etc)
5. When coming back home, take all belongings to a dedicated area where they can be left untouched for few hours. Wash your hands, feet, face with soap properly.
6. Wash masks everyday or every use. Have 2-3 spare masks per person so the can be washed regularly.

## Vaccines

You can track various vaccine research programmes [here](https://www.raps.org/news-and-articles/news-articles/2020/3/covid-19-vaccine-tracker).

Specifically for India the most promising candidate is India's own Covaxin by Bharat Biotech, National Institute of Virology. Early Human trials have been started.

Source: [Covaxin gets clearance for human trails](https://www.indiatvnews.com/business/news-covaxine-coronavirus-vaccine-india-okays-covaxine-for-human-trials-covid-19-patients-dgca-approval-630360)

## Credits

All numbers and graphs are from **[Prof. Shamika Ravi](https://twitter.com/ShamikaRavi/)**. Her daily twitter update is the only update I have followed for last few months and helped me understand a lot about the numbers we see everyday. All charts are from her twitter feed.

Also https://www.covid19india.org/ the only tracker I follow for updates. It has very insightful numbers also a public API to build your own trackers. It is a OpenSource initiative, help them if you can.




