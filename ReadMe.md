
Covid-19 Vaccination project
 =====
 
Introduction and preparation
----

For my project, I will analyze the Covid-19 vaccination data across different countries. Exploratory analysis including summary statistics characterization and data visualization will be performed on the data.
To analyze the data you would need some `R` packages (i.e., "table 1" for the table of summary characteristics; "maps" and "mapdata" for loading map data; "ggplot2" for the figure; "dplyr" for manipulating the data), which can be installed using R commands.

```R
installed_pkgs <- row.names(installed.packages())

pkgs <- c("table1","maps","mapdata","ggplot2","dplyr")

for(p in pkgs){
	if(!(p %in% installed_pkgs)){
		install.packages(p)
	}
}
```


Execute the analysis
------

You can run the command below under the project directory

```
Rscript -e "rmarkdown::render('Vacc_report.Rmd')"
```

This will create a fill named Vacc_report.html in the same folder that contain the results.

