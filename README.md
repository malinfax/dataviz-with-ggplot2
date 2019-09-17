# dataviz-with-ggplot2
For R User Group Malmö~Lund (SkåneR)

## Why does data visualization matter?
- For yourself (analysis): understand your data – see patterns, distribution, identify outliers 
- For others (communication): explain your data, highlight what matters, make it memorable

## What is good data viz?
> ”Graphical excellence is the well-designed presentation of interesting data—a matter of substance, of statistics, and of design … [It] consists of complex ideas communicated with clarity, precision, and efficiency. … [It] is that which gives to the viewer the greatest number of ideas in the shortest time with the least ink in the smallest space … [It] is nearly always multivariate … And graphical excellence requires telling the truth about the data.” (Tufte, 1983, p. 51).

### Good data viz...
- Highlights important aspects of your data
	- Understand your data and know what you want to communicate
- Is informative and easy to understand
	- Know your audience and choose a type of data viz they will understand
	- Don’t try to fit too much information into one viz
	- Before adding flair, ask yourself if it helps explain the data or if you just think it’s cool
- Represents the data without distorting it
	- Always let facts ruin a good story

### Bad data viz can be...
- Misleading 
- Ugly
- Confusing
- Pointless

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

### < DATA >
- The data set you want to visualize!
- Import your data or choose one from the data sets already available
- data() shows you all available data sets from your loaded packages
- R has a built in package called ´datasets´, ggplot2 also comes w/ data sets
- dim(), str(), head(), summary() are good functions to explore your data set
	
### < GEOM_FUNCTION >
- The <GEOM_FUNCTION> is basically the type of plot you want to use. So which one do we want?
- Depends on the data and what we want to explore/show! What’s our question?
	- Numeric? Categoric? Number of variables? Ordered/not ordered? Number of points?
	- Map? Network? Time series?

```r
ggplot(data = diamonds) +
	geom_point(mapping = aes(x = carat, y = price, color = cut))
```
### Picking a color palette
- Consider:
	- Readability: on screen, in print, for people with color blindness, in black and white (the viridis package does a good job of showing why this is important: https://cran.r-project.org/web/packages/viridis/vignettes/intro-to-viridis.html)
	- Continuous or categorical data 

### Other elements to play with
- size
- alpha		
- shape
- fill
- theme  	
- labs():	set title, subtitle, axis labels, legends…
- facet_wrap:	create subplots – super useful! 

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
- What to consider when choosing colors for data visualization: https://blog.datawrapper.de/colors/
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
- Browse the collection of submissions at https://nsgrantham.shinyapps.io/tidytuesdayrocks/ **(look at both viz and code to understand the ggplot structure!)**
- Find a data set that intrigues you
- **Visualize it!** 
	- Choose your own adventure: the good, the bad, or the ugly
	- If you want to, you can copy existing code and play around with it
- Ask for help: we are here to learn from each other
- Share it on twitter using #TidyTuesday if you want

### Extra
- TidyTuesday podcast: https://www.tidytuesday.com/
- Data import cheat sheet: https://www.rstudio.com/resources/cheatsheets/#import
- Data transformation with dplyr cheat sheet: https://www.rstudio.com/resources/cheatsheets/#dplyr
