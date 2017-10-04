**d3heatmap is not actively maintained. You might consider using a newer heatmap package like [heatmaply](https://github.com/talgalili/heatmaply).**

___

# D3 Heatmap for R

This is an R package that implements a heatmap [htmlwidget](http://htmlwidgets.org). It has the following features:

* Highlight rows/columns by clicking axis labels
* Click and drag over colormap to zoom in (click on colormap to zoom out)
* Optional clustering and dendrograms, courtesy of `base::heatmap`

### Example

http://rpubs.com/jcheng/mtcars-heatmap

### Installation

To install:

```r
if (!require("devtools")) install.packages("devtools")
devtools::install_github("rstudio/d3heatmap")
```

### Usage

Like any htmlwidget, you can visualize a d3 heatmap directly from the R console:

```r
library(d3heatmap)
d3heatmap(mtcars, scale = "column", colors = "Spectral")
```

You can also include them in R Markdown chunks, or use them in Shiny applications with the `d3heatmapOutput` and `renderD3heatmap` functions.

See `?d3heatmap` for options.
