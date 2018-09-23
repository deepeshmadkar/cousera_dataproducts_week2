---
title: 'Coursera: Data Product - Week 2'
author: "Deepesh Madkar"
date: "9/23/2018"
output:
  html_document:
    keep_md: true
---



## Location: Mumbai(India)

```r
# Loading Libraries
library(leaflet)

# Passing url of map details
mumbai <- c("<a href= 'https://en.wikipedia.org/wiki/Mumbai' >Mumbai</a>")
mumbaiLat <- 19.07283
mumbaiLong <- 72.88261

# implementing leaflet code
leaflet() %>%
  addTiles() %>%
  # setView(lat = mumbaiLat, lng = mumbaiLong, zoom = 10) %>% 
  addMarkers(lat=mumbaiLat, lng=mumbaiLong, popup = mumbai)
```

<!--html_preserve--><div id="htmlwidget-b0b965165e7d1952cbda" style="width:672px;height:480px;" class="leaflet html-widget"></div>
<script type="application/json" data-for="htmlwidget-b0b965165e7d1952cbda">{"x":{"options":{"crs":{"crsClass":"L.CRS.EPSG3857","code":null,"proj4def":null,"projectedBounds":null,"options":{}}},"calls":[{"method":"addTiles","args":["//{s}.tile.openstreetmap.org/{z}/{x}/{y}.png",null,null,{"minZoom":0,"maxZoom":18,"tileSize":256,"subdomains":"abc","errorTileUrl":"","tms":false,"noWrap":false,"zoomOffset":0,"zoomReverse":false,"opacity":1,"zIndex":1,"detectRetina":false,"attribution":"&copy; <a href=\"http://openstreetmap.org\">OpenStreetMap<\/a> contributors, <a href=\"http://creativecommons.org/licenses/by-sa/2.0/\">CC-BY-SA<\/a>"}]},{"method":"addMarkers","args":[19.07283,72.88261,null,null,null,{"interactive":true,"draggable":false,"keyboard":true,"title":"","alt":"","zIndexOffset":0,"opacity":1,"riseOnHover":false,"riseOffset":250},"<a href= 'https://en.wikipedia.org/wiki/Mumbai' >Mumbai<\/a>",null,null,null,null,{"interactive":false,"permanent":false,"direction":"auto","opacity":1,"offset":[0,0],"textsize":"10px","textOnly":false,"className":"","sticky":true},null]}],"limits":{"lat":[19.07283,19.07283],"lng":[72.88261,72.88261]}},"evals":[],"jsHooks":[]}</script><!--/html_preserve-->

```r
# india_places <- data.frame(name=c("Taj", "Konark", "Hampi", "Pangong", "Hajarduari"),
# 
# rating = c( 2, 4, 1, 3, 5),
# 
# lat=c(27.1750, 19.8876, 15.3350,33.7380,24.1900),
# 
# lng=c(78.0422, 78.0422, 76.4600,79.0075,88.2687))
# 
# my_map <- india_places %>%
# 
# leaflet() %>%
# 
# addTiles() %>%
# 
# addCircles(weight=10, radius=(india_places$rating)*30)
# 
# my_map
```

