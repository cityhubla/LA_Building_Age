![alt text](https://github.com/cityhubla/LA_Building_Age/blob/master/images/builtla_cover.png)
# built : Los Angeles

[LIVE DEMO](http://cityhubla.github.io/LA_Building_Age/)

HTML to load Map tiles from cityhub server host // Breakdown on the processes involved in developing map will be up soon.

Since 2008, there are over 2.9 million buildings in Los Angeles County. This visualization gives an overall look at the age of the building stock as of 2008.
Each building is shaded according to the time they were built. 
Map made with Mapbox Studio and MapboxGL by [Omar Ureta](http://www.theworks.la), inspired by Portland, Oregon: The Age of a City

###Method
* The display of the building outlines with their age was done by linking the two datasets (LARIAC and Local Roll) by their APN (Assessor's Parcel Number). Additionally the street number, name and city were linked through the two datasets.

###Notes
 * Grey areas indicate no data on year building was built.
 * The addresses shown are according to what the 2011 LA County Assessor Roll Data had to the corresponding Parcel Number. Please check with the [LA County APN Property Search](http://maps.assessor.lacounty.gov/GVH_2_2/Index.html?configBase=http://maps.assessor.lacounty.gov/Geocortex/Essentials/REST/sites/PAIS/viewers/PAIS_hv/virtualdirectory/Resources/Config/Default) to verify your address and building age.
 * <b>Please contact me</b> if you intend to use the map as a baselayer for other work. I will be changing the access keys and IP frequently. The intent of posting the code on github is for mappers to understand how this got built with mapbox-gl and the new styling of the features.
 
###Known Inaccuracies
* Building outline data shows what existed in 2008, buildings during the century may have been replaced and is not shown with this map.
* Parcels that have more than one building may contain dates of one of the buildings as the local roll contained only one.
* There are missing dates on buildings even though their date is known through the [LA County APN Property Search](http://maps.assessor.lacounty.gov/GVH_2_2/Index.html?configBase=http://maps.assessor.lacounty.gov/Geocortex/Essentials/REST/sites/PAIS/viewers/PAIS_hv/virtualdirectory/Resources/Config/Default). The data worked with was from the 2011 parcel local roll, a look at the now released 2014 local roll through the County's Open Data portal shows that many have been updated with dates. My apartment for example did not have a date on 2011 local roll and now does on the 2014 set. Updates to the map will reflect the updated set.
* There is a 3 (three) year gap between the Local Roll data (2011) and the Building Outlines (2008). Properties that have new buildings since 2008 will still have the building outline from 2008. The most recent building on the 2011 Local Roll was built in 2009 bringing the gap close to 1 year. The age map will be updated to remove this gap.
* <b>Please report any other inaccuracies in the Issues section of this repo. Many of these can be brought to the attention of LA County and help them improve their datasets.</b>

###From these sources:

  * LARAIC2 and the 2011 LA County Assessor Parcel Local Roll
  * The disclaimer from using these resources are as follows: The data available on this website, including Geographic Information Systems (“GIS”) data, maps, tables, numbers, graphics, and text (hereinafter collectively referred to as the “Information”), is provided AS IS and for you to view, access, copy, distribute and otherwise use the Information at your own risk. The County of Los Angeles, its departments and its affiliated entities, elected and appointed officers, officials, employees and agents (hereinafter referred to as the “County”) make no representation or warranty of any kind regarding this website or Information, explicit or implied.
 
Using this map will ask more questions about LA's development and it should continue to evolve and explore these inquiries. Maps should be [transformative agents](http://www.thepolisblog.org/2010/03/mapping-as-transformative-agent-in.html)

####Help improve this map! 
The building outline data is from 2008, there is a [2014](http://egis3.lacounty.gov/dataportal/2014/10/16/countywide-building-outlines-2014/) set from the county that is not public. An effort is underway to prepare the import of the 2008 buildings and hopefully the 2014 set to [OpenStreetMap](https://github.com/osmlab/labuildings).
