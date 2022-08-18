#Analysis of National UFO Reporting Center Data

##Table of Contents:
##Motivation
##Technologies
##Problems and Challenges

##Motivation
####When I was working in California I had to get up early one morning for work and I saw a UFO.  It made my day.  I was filled with wonder and took that sense of wonder into the day with me.  I was telling everyone that would listen about my experience.  One of my coworkers was very interested in my sighting and as I began to describe it to them, they, somewhat dejectedly, informed me that what I saw was the star-link satellites.  A quick Google search later and my coworkers suspicions were confirmed.  I wanted to examine the self-reported UFO sightings on the National UFO Reporting Center's website (https://nuforc.org) to share in the reporters sense of wonder at seeing the unexplainable and to examine the data to see if I could identify and hotspots for activity or any other information that could increase my odds of seeing a UFO.

##Technologies
####All analysis done in Python 3 within a Jupyter Notebook. All data obtained from National UFO Reporting Center's Index by State(https://nuforc.org/webreports/ndxloc.html) via a webscrape.

##Problems and Challenges
####The webscrape ended up being 51 pages, but 2 pages, for the states of California and Missouri, were unusable due to running into a tag issue within the HTML. Unfortunately, I had to exclude these states from my analysis.  Other problems I ran into were mainly centered around the websites' lack of guidelines while filing a UFO sighting report.  They don't suggest a format to use for the date and time, which led to various discrepancies with that column in my dataframe.  The city column ended up being another one where there was a surprising amount of variability.  'Nashville' will not be counted the same as 'Near Nashville.'  By far the worst offender was the duration column which consisted of everything from 'I dunno a couple minutes' to '1-2 min,' I think I did a decent job at getting a conservative estimate for the mean duration per UFO sighting event in the end.
