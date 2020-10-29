
# Module 2 Final Project - King County House Sales


## Introduction

This project takes a look at the King County House Sales dataset in order to project the cost of homes in King County, Washington. According to research from the [University of Washington](https://www.washington.edu/news/2020/10/15/for-single-adults-and-families-alike-higher-cost-of-living-in-all-washington-counties/), King County is the most expensive area to live in, in terms of cost of living, in Washington state. It is projected that an adult living in King County would need to make at least $44,000 a year in order to get by. The cost of living, however, could double or triple for single parents and multi-family homes. On average, an adult needs to make $17.61 per hour in order to get by. This is alarming, but also not the main objective of this project.

My project is meant to be used as a resource for those seeking to buy a home in King County. The project takes a look at what features directly affect the cost of a home, and projects where the most affordable homes are located within the county. This dataset can be used by low to middle class families seeking to begin a life in King County, or by those seeking to make a profit by flipping a home. In essence, this project is a guide for the home buyer as they naviagte the housing market that is King County. 

This project focuses on three factors in order to determine the cost of living in King's County:
    1. How the location of a home affects it's value.
    1. How the physical attributes of a home (i.e. condition, number of floors, number of bedrooms, etc.) affect the value of the home.
    1. How external factors (i.e. neighbors, grade, year home was built, etc.) where the home is located affect the value of the home.
Using these factors as a basis, families can determine what homes are best suited to their needs.

## Findings

### Location

According to the data, home location has an impact on the price of the home. Homes located in areas such as Seattle, Merer Island, Bellevue, and the surrounding areas are very expensive (in the millions) and would be out of the price range of families seeking affordable homes. Families seeking affordable housing should look towards the southern half of the county, such as Mapple Valley, Hobart, Black Diamond, and southern Seattle. The homes in this area generally cost between a mean price between 230K and 400K, making them affordable for home buyers seeking to start a family in the county. However, majority of these homes are outside of the major city areas, meaning that most home owners will need to commute to work. The maps bellow show the prices of the homes by zipcode and by latitude and longitude loaction.

#### Zipcode's Affect on Home Price
![Housing Price by Zipcode](https://github.com/PNarducci1690/Project_2_KC_Housing_Data/blob/master/King_County_Graphs/Zipcode_Price_Affect_On_Home_Price.PNG)

#### Latitude and Longitude's Affect on Home Price
![Housing Price by longitudinal and latitudinal location](https://github.com/PNarducci1690/Project_2_KC_Housing_Data/blob/master/King_County_Graphs/long_lat_Affect_on_Home_Price.PNG)

### Attributes 

When looking at the attributes of the home, we notice that the square footage (sqft.) of the home has a significant impact on home price. As square footage increases, so does the price of the home. We can see the relationship in the jointplot bellow:

![Sqft_Living Affect on Home Price](https://github.com/PNarducci1690/Project_2_KC_Housing_Data/blob/master/King_County_Graphs/Sqft_living%20Affect%20on%20Home%20Price.PNG)

Most homes in King County have a sqft. between 1k and 2k with a price ranging from as low as 250K up until 500K in value. We also notice that sqft. of a basement (if a basement is present) also brings up the price of the home. We notice in the jointplot below that most basements have a sqft. from 250 to 750 with a price range between 200K to about 600K.

![Sqft Basement Affect on Home Price](https://github.com/PNarducci1690/Project_2_KC_Housing_Data/blob/master/King_County_Graphs/Sqft%20Basement%20Affect%20on%20Home%20Price.PNG)

As we can see, this is concerning because majority of the homes in KC are already priced high at a smaller sqft. value, and most middle class and lower class families will find many of the spacious homes outside of a reasonable price range. We also notice that as the amount of floors, bedrooms, and bathrooms increse in the home, so does the price of the home. Most homeowners seeking a home in Kings County, Washington, can only afford smaller sized homes with fewer floors, bathrooms or bedrooms - which is concerning for working families seeking to start or raise a family in this county. However, homeowners seeking to purchase a home in King County should aim for a "fixer upper" or a home with a condition rating of at most 2, since the homes value will be 300K or less in value.

### External Factors

External factors in our dataset refer to conditions within the homes general vicinity, past, or organizations within KC. We notice, based on our data, that sqft. of the nearest 15 homes plays an important factor on home price. As the sqft of the nearest 15 homes increases, so does the price of the home. We can see this in the jointplot below:

![Sqft of 15 Nearest Neighbors Affect on Home Price](https://github.com/PNarducci1690/Project_2_KC_Housing_Data/blob/master/King_County_Graphs/Sqft%20Nearest%2015%20Neighbors%20Affect%20on%20Home%20Price.PNG)

As we noticed earlier, most homes within the vicinity of the home you are trying to purchase falls between 1000 and 2000 sqft. and raises the price of said home from 200K to almsot 600K. 

We also notice that homes with a waterfront view are out of the purchasing range for lower to middle class families. These homes are priced at around 800K and can go over 1 million in price:

![Waterfront View Affect on Home Price](https://github.com/PNarducci1690/Project_2_KC_Housing_Data/blob/master/King_County_Graphs/Waterfront%20Affect%20on%20Home%20Price.PNG)

These factors limit what neighborhoods and locations families wish to live in in King County, Washington. Forcing homebuyers to move away from urban areas around Lake Washington or other more appealing areas.

However, we notice those seeking to sell homes in King County are at an advantage. According to our data majority of homes in this area were constructed in the 1960s and have continuously gone up in value over the decades. Renovating a home will increase its value, and getting it graded by the King County Housing Organization can possibly double or triple its value if the home is graded at a value of 8 or higher. Howerver, we do notice that the amount of individuals that view a home do decrease its value somewhat. but, as we can see from our data, King County is definitely a sellers market. This makes things difficult for families who are already limited on what they can purchase in the area.

#### Home Grade Affect on Home Value

![Grade Affect on Home Price](https://github.com/PNarducci1690/Project_2_KC_Housing_Data/blob/master/King_County_Graphs/Grade%20Affect%20on%20Home%20Price.PNG)

## Conclusions

Based upon the results of my models, we can infer that King County is a very expensive and over priced area in the Northwest United States. Many homes are outside the affordable range for most families seeking to raise a family and work in the Seattle area. As the size of the home increases, so does the value of the home, forcing home buyers to buy smaller homes at higher prices. However, homeowners in the are who are looking to sell or flip a home should expect to earn money as long as they renovate and increase the grade of their home. 

## Further Research

Other areas of interest with this data set are wheteher or not the following factors affect home price in King County, Washington:
    * Does crime affect housing price in King County?
    * Does time of year determine price values in King County?
    * Does school district play a role in home price?
    * Location to certain areas (financial district, airport, schools, hospitals, etc.) play an important role in home price?