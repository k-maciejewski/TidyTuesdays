# My contributions to TidyTuesdays

## [Horror movies, 2019 week 43](http://rpubs.com/k-maciejewski/545898)

```{r load_data}
horror_movies <- readr::read_csv("https://raw.githubusercontent.com/rfordatascience/tidytuesday/master/data/2019/2019-10-22/horror_movies.csv")
```

```{r data_manipulation}
horror <- horror_movies %>% mutate(id = row_number()) %>% 
  separate_rows(genres, sep = "\\| ") %>% 
  mutate(y = 1) %>%
  spread(genres, y, fill = 0)
horror$filming_country <- gsub(".*, ", "", horror$filming_locations)
worldmap <- map_data("world") %>% tbl_df %>% filter(region !="Antarctica")
```

For my first tidy Tuesday, I explored the [dataset of horror movies](https://github.com/rfordatascience/tidytuesday/tree/master/data/2019/2019-10-22). I'm not a huge horror fan, but when I saw location data, I knew what I would do: practice my mapping! Even though I didn't use it, changing the strings of genres to indicator functions was also good practice.

```{r}
g_film <- horror %>%
  group_by(filming_country) %>%
  summarise(total = n()) %>% 
  top_n(., 5) 
g_film[order(-g_film$total),] %>% knitr::kable()
g1 <- horror %>%
  group_by(release_country) %>%
  summarise(total = n()) %>% 
  top_n(., 5) 
g1[order(-g1$total),] %>% knitr::kable()
g2<-horror %>%
  group_by(release_country) %>%
  summarise(average = mean(review_rating, na.rm = T)) %>% 
  top_n(., 5)
g2[order(-g2$average),] %>% knitr::kable()
```

### Horror movie filming location in each country from 2012 to 2017

![](2019w43/TT_2019_w43-2-1.png)

### Horror movies released by country from 2012 to 2017

![](2019w43/TT_2019_w43-3-1.png)

### Horror movie ratings by country from 2012 to 2017

![](2019w43/TT_2019_w43-4-1.png)
