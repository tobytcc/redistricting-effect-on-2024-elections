# Evaluating the Impact of 2021 Nationwide Redistricting on 2024 US Presidential Elections

**University of Chicago - Machine Learning & Predictive Analytics (ADSP 31009) Final Project**

*Project by Toby Chiu - University of Chicago MS Applied Data Science Student*

All 50 states redrew congressional voting districts in 2021. How will nationwide redistricting efforts affect the presidential election in 2024?

## Introduction

The US votes on presidential elections through a system known as the electoral college, where all 50 states send varying numbers of representatives (depending on population size) to vote for the next president. 

Every ten years, state representatives redraw voting district lines to keep district populations representative of the makeup of actual voters within each district. The federal government mandates that redistricting is done to with equal state legislative representation for all citizens, without discrimination on the basis of race or ethnicity ([Ballotpedia](https://ballotpedia.org/Redistricting) - more info included in link).

However, there is a wealth of evidence to suggest that state lines are often drawn to favor voting outcomes for a party through various techniques, often known as **"Gerrymandering"** ([Brennan Center](https://www.brennancenter.org/our-work/research-reports/gerrymandering-explained)). The [Voting Rights Act of 1965](https://www.archives.gov/milestone-documents/voting-rights-act?_ga=2.99238622.1949216050.1715659324-971477195.1715659323) effectively banned gerrymandering on the basis of reducing the voting power of racial minorities. However, many states effectively bypass this issue by redrawing districts directly based on voting preferences, which often lie closely with racial, socioeconomic, or ethnic makeups across states. [Amos, Gerontakis, and McDonald (2023)](https://esra-conference.org/files/election-science-conference/files/changing_precinct_boundaries_esra-brianamos.pdf) conducted extensive analysis to find that gerrymandered districts often contained more minorities after redistricting on average (a common symptom of "packing" - a gerrymandering tactic), which often led to lower voting turnout than expected.

The most notable example of gerrymandering occurred in 2010, when Republicans donated $30M into "[Project REDMAP](https://www.redistrictingmajorityproject.com/) (Redistricting Majority Project)", pouring large amounts of political funding into winning statewide elections in light-blue swing states with majority Democrat-voting citizens, before severely gerrymandering 10 states in the 2011 redistricting cycle, winning the 2012 US House elections by 33 seats while losing the nationwide popular vote ([The Atlantic](https://www.theatlantic.com/politics/archive/2017/06/how-deep-blue-maryland-shows-redistricting-is-broken/531492/)).

All eligible states redistricted in the 2021 redistricting cycle ([FiveThirtyEight](https://projects.fivethirtyeight.com/redistricting-2022-maps/)). At least 16 states saw legal challenge to their originally proposed redistricting maps ([All About Redistricting](https://redistricting.lls.edu/national-overview/?colorby=Court%20Action&level=Congress&cycle=2020)), with many states still in litigation process just months before the 2024 presidential elections, showing how abundant and hotly-contested gerrymandering practices are across both parties. 

This short video explains gerrymandering in greater detail: [Vox](https://www.youtube.com/watch?v=QZZwoObFMhU&ab_channel=Vox).


## Methodology

#### Partisan Gerrymandering Metric - Efficiency Gap

As data mapping and analytical methods have improved over the years, there have been efforts by many organization to devise metrics and strategies to value the extent of gerrymandering from both parties.

A common technique used in determining the extent of partisan gerrymandering is through the **Efficiency Gap**, developed by Nicholas Stephanopoulos (a UChicago professor!) and Eric McGhee ([Brennan Center](https://www.brennancenter.org/sites/default/files/legal-work/How_the_Efficiency_Gap_Standard_Works.pdf) - an example is given in the paper). The efficiency gap determines the difference in "wasted" votes from both parties in any given area, with wastage defined as: 

<center>
(total winning wasted votes - total losing votes) / total votes
</center>


A completely balanced map should have a zero efficiency gap, with an example 0.20 efficiency gap meaning the winning party won 20% more seats than the voting results would have suggested.

#### Analytical Plan


## Data Sources

## Future Improvements
Other (more advanced) metrics have been created for to quantify partisan gerrymandering from legal ([Stanford Law Review](https://www.stanfordlawreview.org/print/article/three-tests-for-practical-evaluation-of-partisan-gerrymandering/)) and statistical ([Wang, 2016](https://web.math.princeton.edu/~sswang/wang16_ElectionLawJournal_gerrymandering-MD-WI_.pdf), [Princeton Gerrymandering Project](https://gerrymander.princeton.edu/)) standpoints. These metrics may be used to substitute/complement the efficiency gap metric in measuring how and to what extent gerrymandering plays a part in presidential elections.