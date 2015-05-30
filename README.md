![alt text](https://github.com/cityhubla/LA_Building_Age/blob/master/images/builtla_cover.png)
# built : Los Angeles

[LIVE DEMO](http://cityhubla.github.io/LA_Building_Age/)

HTML to load Map tiles from cityhub server host // Breakdown on the processes involved in developing map will be up soon.

Since 2008, there are over 2.9 million buildings in Los Angeles County. 
Each building is shaded according to the time they were built. 
Map made with Mapbox Studio and MapboxGL by [Omar Ureta](http://www.theworks.la), inspired by Portland, Oregon: The Age of a City

Notes

 * Grey areas indicate no data on year building was built.
 * Building outline data shows what existed in 2008, buildings during the century may have been replaced and is not shown with this map.
 * Due to the tremendous size of the two datasets, Almost 2 Gigabytes!! A sole i7 took many hours crunching the data to magically display what you see, there will be inaccuracies but this map does help paint a good picture of how Los Angeles has grown through the animation. For example the parcel data I worked with was made in 2011, the building where I live has no "year built," the recently published 2014 parcel dataset now has it at 1914, which means that many buildings of this current map do really have dates. Future updates to this map will reflect these kinds of descrepancies.
 * <b>Please contact me</b> if you intend to use the map as a baselayer for other work. I will be changing the access keys and IP frequently. The intent of posting the code on github is for mappers to understand how this got built with mapbox-gl and the new styling of the features.

From these sources:

  * LARAIC2 and the 2011 LA County Assessor Parcel Local Roll
 
Using this map will ask more questions about LA's development and it should continue to evolve and explore these inquiries. Maps should be [transformative agents](http://www.thepolisblog.org/2010/03/mapping-as-transformative-agent-in.html)
