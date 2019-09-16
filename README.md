# dataviz-with-ggplot2
For R User Group Malmö~Lund (SkåneR)

## The anatomy of a ggplot2:
```r
install.packages(ggplot2) # First time using the package: install
library(ggplot2) # Load the pkg

ggplot(data = <DATA>) + 
	<GEOM_FUNCTION>(mapping = aes(<MAPPINGS>)) +
	...

# You can also put the aes() in ggplot():

ggplot(data = <DATA>, mapping = aes(<MAPPINGS>)) + 
	<GEOM_FUNCTION>() +
	...
```

## Resources:


### Free online books:
- ggplot2: Elegant Graphics for Data Analysis – Hadley Wickham (https://ggplot2-book.org/)
- Data Visualization: A Practical In
troduction – Kieran Healy (http://socviz.co/)
- R for Data Science – Garrett Grolemund & Hadley Wickham (https://r4ds.had.co.nz/)
- Fundamentals of Data Visualization – Claus O. Wilke (https://serialmentor.com/dataviz/)
- ggplot2 cookbook by Winston Chang (http://www.cookbook-r.com/Graphs/)

### ggplot2 reference and cheatsheet:
- https://ggplot2.tidyverse.org/reference/index.html
- https://www.rstudio.com/resources/cheatsheets/#ggplot2

### Types of graphs:
- From Data to Viz: https://www.data-to-viz.com/
- R Graph Gallery: http://r-graph-gallery.com/
- Top 50 ggplot2 visualizations – The Master List (with Full R Code): http://r-statistics.co/Top50-Ggplot2-Visualizations-MasterList-R-Code.html

### Color palettes:
- Your Friendly Guide to Colors in Data Visualization: https://blog.datawrapper.de/colorguide/
- Comprehensive list of color palettes in R: https://github.com/EmilHvitfeldt/r-color-palettes
- The viridis color palettes: https://cran.r-project.org/web/packages/viridis/vignettes/intro-to-viridis.html
- The paletteer gallery: https://github.com/PMassicotte/paletteer_gallery

### Themes:
- https://ggplot2.tidyverse.org/reference/ggtheme.html
- hrbrthemes: https://github.com/hrbrmstr/hrbrthemes
- Customizing theme and legends: http://r-statistics.co/Complete-Ggplot2-Tutorial-Part2-Customizing-Theme-With-R-Code.html

### facet_wrap():
- https://www.sharpsightlabs.com/blog/facet_wrap/

### ggplot2 extensions gallery:
- http://www.ggplot2-exts.org/gallery/
- **Browse this!** Find more color palettes, themes, additional types of plots… 

### Community: 
- R for Data Science Online Learning Community: https://www.rfordatasci.com/
- RStudio Community: https://community.rstudio.com/
- Data Visualization Society: https://www.datavisualizationsociety.com/
- Twitter: #rstats #dataviz #TidyTuesday

## #TidyTuesday
- Browse the data sets posted at 
https://github.com/rfordatascience/tidytuesday
- Browse the collection of submissions at https://nsgrantham.shinyapps.io/tidytuesdayrocks/
- Find a data set that intrigues you
- **Visualize it!** 
- Ask for help: we are here to learn from each other
- Share it on twitter using #TidyTuesday if you want

