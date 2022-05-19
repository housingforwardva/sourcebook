# Sourcebook

## About Sourcebook

This is the repository for Sourcebook, a collection of interactive dashboards for data on housing affordability. Sourcebook is built by [HousingForward Virginia](https://www.housingforwardva.org), a nonprofit organization helping housing practitioners, government officials, and advocates advance better housing opportunities across the Commonwealth.

Housing and housing-related data is spread across multiple sources and can be time-consuming to clean up, analyze, and visualize. Sourcebook brings together the most important data points in one place to make that work simpler for you.

The current publicly available version of Sourcebook is at [housingforwardva.org/toolkits/sourcebook](https://www.housingforwardva.org/toolkits/sourcebook).

## How this repository is organized

### Main directory

The main Sourcebook directory includes an administrative `00-admin` folder, along with seven folders for each data topic. These include:

* Demographic trends (`10-demographics`)
* Income and employment indicators (`20-economic`)
* Housing inventory trends (`30-inventory`)
* Homeownership and for-sale market (`40-homeownership`)
* Rental market (`50-rental`)
* Housing affordability measures (`60-affordability`)
* Homelessness and housing instability (`70-instability`)

### Data topic subfolders

Within each of these category folders are subfolders containing the data and documentation for each page in Sourcebook. Each of these subfolders begin with two-digit number corresponding with the category range and ends with short title of the data topic.

For example, the path for the home sales price page is `40-homeownership/42-home-sales`.

### Page subfolder contents

Every subfolder contains the data, scripts, visualizations, and output files needed to produce that page on the HousingForward Virginia website.

* `/raw` contains any manually collected and unaltered datasets
* `/data` contains cleaned .csv files produced by the R scripts and used by Tableau dashboards
* `/tableau-extracts` contains Tableau Extract .hyper files to support publishing to Tableau Public
* At least one .Rmd file documenting data collection, prep, and export (with associated knitted .html)
* One .Rmd file containing the content to be uploaded to the Sourcebook webpage (with associated knitted .html)
* At least one .twb Tableau Workbook file used to build the dashboard(s)


## Methodology

HousingForward Virginia currently uses a wide array of R scripts to collect and organize data. Data is then visualized using Tableau and published to our [Tableau Public](https://public.tableau.com/app/profile/housingforward.virginia/) profile.

## Sponsors and acknowledgements

Sourcebook is made possible with the support of:

* Atlantic Union Bank
* Virginia REALTORS®
* Wells Fargo
* Virginia Housing

HousingForward Virginia is also very thankful for the invaluable technical assistance provided by [Kyle Walker](https://github.com/walkerke), along with the [Virginia Center for Housing Research](http://vchr.vt.edu/) for laying Sourcebook's initial foundation a decade ago.
