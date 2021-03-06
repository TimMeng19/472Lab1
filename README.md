# 472Lab1 - Haotian Meng



## 1. A screenshot of the web map:

[logo]: https://github.com/TimMeng19/472Lab1/blob/main/Screenshot%20-%20Web%20Map.png "Screenshot of the map"
![alt text][logo]
##  2. The Github Pages link to the web map
https://timmeng19.github.io/472Lab1/map.html

The Mapbox style file can be found in the main page of this repo

## 3. The Reflective Analysis and associated references

  As one of the most popular types of event, modern professional sports have been paid extensive attention by the society. The World Cup, the NBA, the Premier League and many other kinds of sport events attract millions of fans to participate and watch games. While the influence of sports events does not only remain in the society level, but it also brings significant economic benefits to local communities. Sport events improve local economic prosperity to a city on the basis of well-developed sports related infrastructures (Baade & Dye, 1988). In the web-map created in this lab, the purpose is to examine this claim and aim to find out possible correlation between sport events and local economies in the United Kingdoms. The audience for this map includes city planners, government officials and other decision makers in urban planning.

  The United Kingdoms is selected to be the study area in this map. The reason of doing so is because professional sports leagues have been developed over a century in the UK, some famous leagues/events such as the Premier League, and the Championships, Wimbledon are all well-known worldwide and have brought enormous commercial benefits to other local business (Millward, 2013). Therefore, it is reasonable to select the UK as the study area given its developed environment for sport events and enthusiasm. For the main dataset, the location of stadiums is used because a stadium is the core element to sport events among all infrastructures, and its location can be considered as the center of economic radiation of sport events. This data is initially retrieved from a Wikipedia page and then verified via official pages for all stadiums. The other dataset used in this map is the Gross Disposable Household Income (GDHI) in year 2006 and 2016 in the Great Britain. This dataset is retrieved from the Ministry of Housing, Communities and Local Government, and it simply shows the amount of money that citizens get after income distribution measures, which can directly affect the economic status change for households in the county level. 

  To show the customized data layers - one point feature layer and two polygon feature layers - I used several styling methods in both the Mapbox Studio and Mapbox GL JS to refine the map. Firstly, in Mapbox Studio, since it is the first time I use Mapbox, I designed most of the map elements based on suggestions from The Guide to Map Design written by Amy Lee. To begin with, the focus of this map is the three customized layers chosen, so I selected the Monochrome style base-map, which shows basic map elements (roads, land uses) but does not highlight them. This can be helpful for the audience to view the customized data and learn about local conditions at the same time. For the color hierarchy, two color schemes were applied to the stadium layer and the GDHI layer. A qualitative color scheme was used to show different kinds of stadium, and a sequential color scheme was used to map out the GDHI data classes. Color difference for both layers was being considered as well, so that one can easily differentiate and identify features. Typographic hierarchy was also considered for the customized layers. Names for each stadium were changed to Quintessential font and brown color in order to distinguish them from other administrative labels. Also, for the scale hierarchy aspect, these labels would not be displayed when the zoom level is not larger than 7. I applied this rule because the overall distribution of the 154 stadiums is quite clustered given the fact that the UK is relatively a small country. Therefore, to avoid map elements crowded together, this zoom level rule was applied. Moreover, due to this reason, several other features including text offset, labels size, point size and layer opacity are all applied with zoom level rules for a better visualization at different zoom levels. 
  
  After using the Mapbox Studio, I used the Mapbox GL JS and Atom.io to further enhance this map. To let the audience view the map more intuitively, I think map interactivity is very crucial. Firstly, I created some basic interactive elements for the map, such as the title and legends to provide basic information. Beside these basic functions, I then built a hover function and a popup function for the stadium points to let viewers see the detail information such as the capacity and located city/town for a certain stadium. I also created two toggles for showing or hiding the two GDHI layers for year 2006 and 2016. I believe this enables viewers to compare the GDHI changes as well as see map elements and data clearer at different zoom level. Lastly, I created a button which can take viewers back to the original extent. This is helpful to those who are unfamiliar with the geography of the UK, and can redirect them back to the right place. 

  In conclusion, I used Mapbox Studio to style basic elements and then used Mapbox GL JS, Atom.io and the HTML programming language to build interactivity and complete this web map. To further improve my map, inserting an image of each stadium into each popup window can bring a better sense to viewers about each stadium feature. I tried to reach this goal, however, I failed since I am not able to retrieve image from the Internet to the local hosted webpage. Another enhancement I can make in the future is to change the qualitative stadium point data to a proportional symbol layer with the stadium capacity being the value, and still represents the same qualitative data (stadium type). Afterall, there are still many places could be enhanced better in this map.

Reference:

1. Baade, R. A., & Dye, R. F. (1988). Sports stadiums and area development: A critical review. Sage Publications. https://doi.org/10.1177/089124248800200306

2. Millward, P. (2013). New football directors in the twenty-first century: Profit and revenue in the english premier league's transnational age. Leisure Studies, 32(4), 399-414. https://doi.org/10.1080/02614367.2012.673130

3. Lee, A. (2021). The Guide to Map Design. Mapbox. https://go.mapbox.com/rs/117-NXK-490/images/the-guide-to-map-design.pdf


Data Source:
https://data-communities.opendata.arcgis.com/datasets/household-income?geometry=-86.580%2C46.098%2C80.676%2C63.486&selectedAttribute=Y_2016

