# README 

Welcome to this Git repository containing a Tutorial for HYD273 students: Introduction to Geostatistics: Statistical treatment of spatial data with hydrologic emphasis. Topics include: theory of random functions, variogram analysis, Kriging/co-Kriging, indicator geostatistics, and stochastic simulation of spatial variability.

Special thanks and major credit to Hijmans, R. (2016) Interpolation [Source code] http://www.rspatial.org for cleaned up example data and starter code. 

Table of Contents: 

1.0 Spatial Data  
2.0 Blank Interpolation Zone  
3.0 Evaluation Metrics  
4.0 The Average Model  
5.0 Inverse Distance Weighted Model  
6.0 Variogram  
    .... 6.1 Anisotropy  
7.0 Kriging Models  
    .... 7.1 Simple Kriging  
    .... 7.2 Ordinary Kriging  
    .... 7.3 Universal Kriging  
    .... 7.4 Indicator Kriging   
    .... 7.5 Local Kriging  
    .... 7.6 CoKriging  
    .... 7.7 Block Kriging  
8.0 Sequential Gaussian Simulation  
9.0 Comparing Models  
    .... 9.1 Comparing RMSE   
    .... 9.2 Comparing Plots  
10.0 Ensemble Model  
11.0 Transition Probability Markov Chain 

## Execution
This repository contains an R Markdown file that you can use to analyze data or create reports. To use the R Markdown file, you need to have the following:

1. R installed on your computer
2. RStudio (an integrated development environment for R) installed on your computer
3. The necessary R packages installed on your computer

## Installation

### 1. Install R

If you haven't already done so, please download and install R from the following website:

https://cran.r-project.org/

### 2. Install RStudio

Once you have installed R, you should then download and install RStudio from the following website:

https://www.rstudio.com/products/rstudio/download/

### 3. Install the necessary R packages

To run the R Markdown file, you will need to install the following packages:

- `sp`
- `rgdal`
- `raster`
- `gstat`
- `dismo`
- `spMC`
- `knitr`
- `rmarkdown`

To install these packages, open RStudio and run the following commands in the console:

```
# Install the necessary packages
install.packages("sp")
install.packages("rgdal")
install.packages("knitr")
install.packages("rmarkdown")
``` 

You can customize the package list as per your requirements. Simply include this code block in your markdown file, and the packages will be installed when the code is executed.

## Usage

### 1. Download the R Markdown file

You can download the R Markdown file from this Git repository by clicking on  "<>Code" then "Download ZIP" or by cloning the repository using the following command:

```
git clone https://github.com/whiteellie/geostatistics-tutorial.git
```

### 2. Open the R Markdown file in RStudio

Once you have downloaded the R Markdown file, open it in RStudio by navigating to the file location and double-clicking on the file.

### 3. Run the R Markdown file

You can run the R Markdown file by clicking on the "Knit" button in RStudio, or by running the following command in the console:

```
rmarkdown::render()
```

## Repo Organization
* See the results in `Tutorial.html` or `Tutorial.pdf`.
* The code is included in `Tutorial.rmd` file.
* `airqual.csv` has the ozone data used in the Tutorial.
* `inputdata/counties/` includes California county shapefiles for plotting purposes.
* The `papers/` folder includes some useful papers found online for further reading.

## Further Improvements Needed:
* include spatio-temporal kriging in the analysis
* apply the transision probability markov chain analysis to a better dataset

## My sessionInfo()
R version 4.2.3 (2023-03-15 ucrt)
Platform: x86_64-w64-mingw32/x64 (64-bit)
Running under: Windows 10 x64 (build 19045)

Matrix products: default

locale:
[1] LC_COLLATE=English_United States.utf8  LC_CTYPE=English_United States.utf8    LC_MONETARY=English_United States.utf8
[4] LC_NUMERIC=C                           LC_TIME=English_United States.utf8    

attached base packages:
[1] stats     graphics  grDevices utils     datasets  methods   base     

other attached packages:
[1] spMC_0.3.15        RColorBrewer_1.1-3 dismo_1.3-9        gstat_2.1-1        raster_3.6-14      rgdal_1.6-4       
[7] sp_1.6-0          

loaded via a namespace (and not attached):
 [1] Rcpp_1.0.10      rstudioapi_0.14  knitr_1.42       lattice_0.20-45  FNN_1.1.3.2      rlang_1.0.6      fastmap_1.1.0   
 [8] tools_4.2.3      xts_0.12.2       grid_4.2.3       xfun_0.36        terra_1.7-3      cli_3.6.0        htmltools_0.5.4 
[15] intervals_0.15.3 yaml_2.3.7       digest_0.6.31    codetools_0.2-19 evaluate_0.20    rmarkdown_2.20   compiler_4.2.3  
[22] spacetime_1.3-0  zoo_1.8-11 

## Conclusion
Thank you for using this Git repository! We hope that you find the R Markdown file useful for your data analysis or report writing needs. If you have any questions or feedback, please feel free to contact me white.elaheh@gmail.com.