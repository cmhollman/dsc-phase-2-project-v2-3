![Header](https://github.com/cmhollman/dsc-phase-2-project-v2-3/blob/main/Images/stock_image_house.jpg)



# King County Housing Analysis

**Author**: [Chris Hollman](mailto:chollman91@gmail.com)

## Overview

This project analyzes housing data in King County. A real estate group in the area is investing in physical ads targeting potential home sellers. The goal of this project is to model the available data and use it to help guide the group's marketing team as to where to focus these ads. 

## Business Problem

A real estate group is looking to represent homeowners who would like to sell their homes. In order to maximize the impact of their ads, we are investigating which zipcodes are associated with higher value homes. For the larger ads, we are investigating other factors that increase the price of a home so that larger ads can be placed in areas where these features are most often found.  

## Data

The data for this project comes from one dataset which is included in this repository:
data/kc_housing_data.csv
This data contains information from over 21,5000 homes sales including price, square footage, overall conditon, quality, and year built. There are also columns for zipcodes, which will be our main focus.  

## Methods

This project uses multiple linear regression to model the data. This will allow us to gain insight into which variables influence the price of a home and how. 

## Results

The zipcodes most associated with increased house prices were 98005(Bellevue), 98112(Washington Park Area) and 98102(Capitol Hill)
The zipcode used for reference is 98070(Vashon Island) as average home sales here are close to the average sale price in the dataset as a whole. Houses in Belleview sell for 72% more, Washinton Park houses sell for 57% more, and Capitol hill houses sell for 55% more. Also noteworthy, waterfront properties are associated with a 36% increase in price.

The sales for these target zipcodes are plotted in red on the chart below.

![zip_date_plot]https://github.com/cmhollman/dsc-phase-2-project-v2-3/blob/main/Images/zipode_plot.png


## Conclusions

This analysis leads to the following recommendations for advertising strategy:

- **Focus mailings in zipcodes with higher house prices.** These areas are higly desirable to live in, and will generate higher commissions if the mailings attract any new clients.
- **Place largers ads near waterfront areas.** Some of the larger ads should be positioned along roads that lead in and out of residential areas with waterfront properties. Waterfront areas tend to attract more foot traffic in general and these billboards should be placed where potential sellers who own waterfront properties will be more likely to see them.

### Next Steps

Further analyses could provide more insight into the King County housing market:

- **Reintroduce latitude and longitude.** Plotting home sales by their coordinates could reveal smaller pockets of increased home values throughout King County. This could provide more specific target areas.
- **Look into number of sales in each zipcode.** A complimentary strategy to chasing high value sales is to focus on areas with higher housing turnover. This could lead to better success rates for mailed advertising. 
- **Model improvement** Our model is still being influenced by outlier data and can be improved. This may involve splitting the data into multiple subsets in order to more accurately model each "tier" of sales. 

## For More Information

See the full analysis in the [Jupyter Notebook](https://github.com/cmhollman/dsc-phase-2-project-v2-3/blob/main/kc_notebook.ipynb) 

or review this [presentation](https://github.com/cmhollman/dsc-phase-2-project-v2-3/blob/main/King_County_Slides.pdf).

For additional info, contact Chris Hollman at [chollman91@gmail.com](mailto:chollman91@gmail.com)


## Repository Structure

```
├── data
├── Images
├── kc_notebook.ipynb
├── CONTRIBUTING.md
├── King_County_Slides.pdf
├── LICENSE.md
└── README.md