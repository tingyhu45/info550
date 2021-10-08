
My project

For my project, I will analyze the Covid-19 vaccination data across different countries.Exploratory analysis including characterizing summary statistics and data visualization will be performed on the data.
To analyze the data you would need to some R packages, which can be installed using R commands.

installed_pkgs <- row.names(installed.packages())
pkgs <- c("maps", "mapdata","ggplot2","dplyr")
for(p in pkgs){
	if(!(p %in% installed_pkgs)){
		install.packages(p)
	}
}


Execute the analysis

You can run the command below under the project directory

Rscript -e "rmarkdown::render('vacc_report.Rmd')"

This will create a fill named vacc_report.html in the same folder that contain the results.

