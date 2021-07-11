# hawl

New plan:
1. Make handcrafted data set, no reliance on api. 
2. Show the chart
3. Have custom elements on the page to filter listed people by XYZ.
4. Make the json into sql to show relations between people

Timeline of scholars, empires and events from history (Arabic, then English)

Google charts (https://developers.google.com/chart/interactive/docs/gallery/timeline) seems best option, though D3 was tempting. Other libraries don't support timelines

Must use hijra date native: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Intl/DateTimeFormat

Arabic first then English

For information… should get a proper book. Wikipedia can do till then

For data, let's start with CSV since it's easy to handle, then convert into a JSON to feed into the codebase



# The nativr data format:
*The aim is to increase historical awareness and knowledge, in an easy to understand and quick to use way.*

*Its better to collect more data and not use, than to need more information later and rush to find it*

Data types: event, era, person

Properties for each type (required are starred):

Event: Name*, date*, region*, effect (calamity, blessing, neutral), blurb

Era: Name*, start year*, end year*, region*, blurb

Person: Name*, birth year*, death year*, region of birth*, regions of life (array: location, arrival, departure), fields, affiliation, blurb, peers (array: relation to other persons), teachers, students 
