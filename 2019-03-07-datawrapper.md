---
title: "Datawrapper"
date: 2019-03-07
---

https://www.datawrapper.de/

Key selling points:

- Export graphics for print!
- Free for under $50k pageviews; $115/year afterwards according to one audience member (and you can share a login across a newsroom)
- No approval required from corporate since you don't need to install software.

The exercises:

1. From https://data.fivethirtyeight.com/ download the `nfl-fandom` data set, unzip it.
2. On Google Sheets, import the "surveymonkey" CSV from that data.
	1. Remove the top row.
	2. Remove all columns except the independent, GOP, and democrat.
	3. find-and-replace to remove all `%` signs. Datawrapper prefers to operate without units in the source data.
	3. Click "Share" to get the share link and set the visibility to "Anyone with link" or "Public on Internet".
	4. Copy the link.
3. In Datawrapper, create a new chart, choose the "from Google Sheet" option, and paste your URL. Because you're using a Google Sheet, edits made in the sheet will be reflected in Datawrapper whenever you edit or republish the chart.
	1. Walk through the "check and describe" tab to make sure the data is correct.
	2. In the "visualize" tab, make what changes you need.
	3. Publish the chart.
	4. Realize you need to make some changes. Go back to the "Visualize" tab and make those changes, then walk forward through the tabs to "Publish and Embed" and re-publish the chart.

Here's what I made:

<iframe title="Chart: NFL fanbases by party identification" aria-describedby="SurveyMonkey data was derived from a poll of American adults ages 18 and older, conducted between Sept. 1-7, 2017.Listed numbers are the raw totals for respondents who ranked a given NFL team among their three favorites, and how many identified with a given party (further broken down by race). We also list the percentages of the entire sample that identified with each party, and were of each race." id="datawrapper-chart-X9hXA" src="//datawrapper.dwcdn.net/X9hXA/2/" scrolling="no" frameborder="0" style="width: 0; min-width: 100% !important;" height="1027"></iframe><script type="text/javascript">!function(){"use strict";window.addEventListener("message",function(a){if(void 0!==a.data["datawrapper-height"])for(var t in a.data["datawrapper-height"]){var e=document.getElementById("datawrapper-chart-"+t);e&&(e.style.height=a.data["datawrapper-height"][t]+"px")}})}();</script>

Besides charts, Datawrapper does maps as well, but the number that can be made is limited for free accounts.
