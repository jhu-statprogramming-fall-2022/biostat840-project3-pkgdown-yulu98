# RColorBrewer

The goal of RColorBrew is to provide color schemes for maps (and other graphics) designed by Cynthia Brewer as described at http://colorbrewer2.org.

# Author

Erich Neuwirth, University of Vienna, erich.neuwirth@univie.ac.at


## List of functions

1.  [brewer.pal] - ColorBrewer palettes
2.  [display.brewer.all] - ColorBrewer palettes
3.  [display.brewer.pal] - ColorBrewer palettes

## Original GitHub Link

https://github.com/yulu98/RColorBrewer.git

## Customization of Website

1. Changed the visual style of the site with bootswatch
2. Detailed customized the visual style using bslib corrected the height
3. Detailed customized the visual style using bslib customized color
4. Added a custom articles menu using navbar
5. Added a footer


## Example

This is a basic example which shows you how to solve a common problem:

``` r
## create a sequential palette for usage and show colors
mypalette<-brewer.pal(7,"Greens")
image(1:7,1,as.matrix(1:7),col=mypalette,xlab="Greens (sequential)",
       ylab="",xaxt="n",yaxt="n",bty="n")
## display a divergent palette
display.brewer.pal(7,"BrBG")
devAskNewPage(ask=TRUE)
## display a qualitative palette
display.brewer.pal(7,"Accent")
devAskNewPage(ask=TRUE)
## display a palettes simultanoeusly
display.brewer.all(n=10, exact.n=FALSE)
devAskNewPage(ask=TRUE)
display.brewer.all(n=10)
devAskNewPage(ask=TRUE)
display.brewer.all()
devAskNewPage(ask=TRUE)
display.brewer.all(type="div")
devAskNewPage(ask=TRUE)
display.brewer.all(type="seq")
devAskNewPage(ask=TRUE)
display.brewer.all(type="qual") 
devAskNewPage(ask=TRUE)
display.brewer.all(n=5,type="div",exact.n=TRUE)
devAskNewPage(ask=TRUE)
display.brewer.all(colorblindFriendly=TRUE)
devAskNewPage(ask=TRUE)
brewer.pal.info
brewer.pal.info["Blues",]
brewer.pal.info["Blues",]$maxcolors
```
