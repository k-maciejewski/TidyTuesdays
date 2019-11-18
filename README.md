# My contributions to TidyTuesdays

## [Horror movies, 2019 week 43](https://k-maciejewski.github.io/TidyTuesdays/2019w43/TT_2019_w43.html)

Link to dashboard above, see folder for code and more.

For my first tidy Tuesday, I explored the [dataset of horror movies](https://github.com/rfordatascience/tidytuesday/tree/master/data/2019/2019-10-22). 

### Horror movie filming location in each country from 2012 to 2017

![](2019w43/TT_2019_w43-2-1.png)

### Horror movies released by country from 2012 to 2017

![](2019w43/TT_2019_w43-3-1.png)

### Horror movie ratings by country from 2012 to 2017

![](2019w43/TT_2019_w43-4-1.png)


## [SQUIRREL!! 2019 week 44](https://k-maciejewski.github.io/TidyTuesdays/TT_2019_44.html)

Link to page above, see folder for code and more.

This tidy tuesday explores the [squirrel census!](https://www.thesquirrelcensus.com). I took the opportunity to try to learn a little [Leaflet.](https://leafletjs.com)

The first map shows all squirrels with given distance above ground at which they were sighted. NA's were filtered out. According to [the data dictionary](https://github.com/rfordatascience/tidytuesday/tree/master/data/2019/2019-10-29#data-dictionary), fields were populated with a value of “FALSE” if the squirrel was on the ground plane so these values were changed to zeros. This map is mostly filled with dark blue, the color of ground-dwelling squirrels.

### All squirrels

![](2019w44/Map1.png)

### Heights below 50, and above ground level

![](2019w44/Map2.png)

### Heights above 50 

![](2019w44/Map3.png)

## [Walk or Bike to work](https://k-maciejewski.github.io/TidyTuesdays/TT_2019_45.html)

This week is [Modes Less Traveled - Bicycling and Walking to Work in the United States: 2008-2012](https://github.com/rfordatascience/tidytuesday/tree/master/data/2019/2019-11-05) from the  [ACS](https://www.census.gov/library/publications/2014/acs/acs-25.html?#).

The `commute.csv` dataset on Github was tidied from 6 raw excel files. The code and final dataset was already provided.

### Box plots of mode of transport, by city size and US region

![](TT_2019_45_files/figure-html/plots-1.png)

### Maps of walk or bike, coloring by city average and state average

![](TT_2019_45_files/figure-html/maps-1.png)

![](TT_2019_45_files/figure-html/maps-3.png)