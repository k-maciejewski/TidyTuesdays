# My contributions to TidyTuesdays

## [Horror movies, 2019 week 43](http://rpubs.com/k-maciejewski/545898)

Link to R-Pub above, see folder for code and more.

For my first tidy Tuesday, I explored the [dataset of horror movies](https://github.com/rfordatascience/tidytuesday/tree/master/data/2019/2019-10-22). I'm not a huge horror fan, but when I saw location data, I knew what I would do: practice my mapping! Even though I didn't use it, changing the strings of genres to indicator functions was also good practice.

### Horror movie filming location in each country from 2012 to 2017

![](2019w43/TT_2019_w43-2-1.png)

### Horror movies released by country from 2012 to 2017

![](2019w43/TT_2019_w43-3-1.png)

### Horror movie ratings by country from 2012 to 2017

![](2019w43/TT_2019_w43-4-1.png)


## [SQUIRREL!! 2019 week 44](http://rpubs.com/k-maciejewski/547777)

Link to R-Pub above, see folder for code and more.

This tidy tuesday explores the [squirrel census!](https://www.thesquirrelcensus.com) Obviously, the data needed to be mapped, so I took the opportunity to try to learn a little [Leaflet.](https://leafletjs.com)

The first map shows all squirrels with given distance above ground at which they were sighted. NA's were filtered out. According to [the data dictionary](https://github.com/rfordatascience/tidytuesday/tree/master/data/2019/2019-10-29#data-dictionary), fields were populated with a value of “FALSE” if the squirrel was on the ground plane so these values were changed to zeros. This map is mostly filled with dark blue, the color of ground-dwelling squirrels.

### All squirrels

![](2019w44/Map1.png)

### Heights below 50, and above ground level

![](2019w44/Map2.png)

### Heights above 50 

![](2019w44/Map3.png)
