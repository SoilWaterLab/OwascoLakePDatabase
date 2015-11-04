# OwascoLakePDatabase
This repository contains the sample event data with a special focus on phosphorus (P) for a number of sites located within the Owasco Lake Watershed (OLW).  In addition to the database itself, this repository also contains example R scripts that can be used as a template to query the data.


## Contact Information ##
Author: Sheila Saia

Email: sms493@cornell.edu

Updated: November 4, 2015


## OLW Phosphorus (P) Database Description ##

The associated Excel file (OLW_P_database.xlsx) contains tabs for various pieces of the database that can be saved as text files and used in conjunction with the example R script also provided (OwascoPDatabase_ExampleQueryScript.R).  The text files coresponding to the different tabs in the Excel file are located in the 'TextFiles' folder.  These data include information on the site location (Site_Info.txt) and the sampling events (Sample_Data.txt).  The third text file (File_Info.txt) is needed to read the site location and sampling event data into R.


## Using the Eample Query Script ##

To use the eample query script, you must download all the OwascoLakePDatabase files on your computer.  In order to read in the text files you must update the working directory of your R script.  To do this you can right click on the TextFiles folder on your computer and click on 'Properties'.  The file path should be given and this should be copied into the setwd() command in the example R Script.  Be sure to change '\' to '//' for R processing purposes.  If my friend Chelsea wanted to run the example query script from data on her Desktop she would replace 

setwd('C://Users//Sheila//Documents//Cornell//CodeRepository//Owasco_Lake_P_ Database//OwascoLakePDatabase//TextFiles')

with... 

setwd('C://Users//Chelsea//Desktop//OwascoLakePDatabase//TextFiles')

To run the example query script you will also have to install the sqldf package in R.  To do this you can go to Packages>Install Packages... in R.  Choose your CRAN mirror.  For example USA PA is close to Ithaca so I'll choose that mirror.  Then you can find and install the sqldf package.

More info on the sqldf package can be found at: [https://cran.r-project.org/web/packages/sqldf/sqldf.pdf](https://cran.r-project.org/web/packages/sqldf/sqldf.pdf) . For reference sqldf uses SQLite.

## Licensing ##

Please be sure to contact Sheila Saia at sms493@cornell.edu if you use or modifiy any aspects of this program or find any errors.  the Owasco Lake Watershed P Database is made available under the Open Data Commons Attribution License: http://opendatacommons.org/licenses/by/1.0.  For the human readible version of the Open Data Commons Attribution License: [http://opendatacommons.org/licenses/by/summary/](http://opendatacommons.org/licenses/by/summary/).