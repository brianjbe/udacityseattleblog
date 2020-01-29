## Seattle Airbnb Analysis

## Table Of Contents

1. [Installation](#installation)
2. [Concept](#concept)
3. [Files](#files)
4. [Data Decisions](#decisions)
5. [Results](#results)


## Installation <a name=installation></a>

This project requires no additional software outside of the base Anaconda Python distribution.  The version of Pandas must be at least 0.25.3,

## Concept <a name=concept></a>

The concept behind this project was to analyze the data from Inside Airbnb to determine if there were any price patterns related to seasonality, location, and unit size.

## Files <a name=files></a>

The data files are included under the seattle subfolder.  All data and regression analysis is contained in the main .py file.

## Data Decisions <a name=decisions></a>

Actual reservation data is not available within this data set which makes it difficult to actually know how many units were actually rented.  For this reason I did not try to determine how likely a unit was to be rented.  I did use the review data as a baseline for what the busiest times of year are which lined up with the price increases and unit availability.

In order to use this data in an actual model the following steps were taking to clean up the data:

1. Dropped all of the empty columns including Square Feet.
2. Converted string price fields into actual float values.
3. Filled review fields in with mean values.
4. Converted string date fields into actual dates and date part fields such as month and day of week.
5. One Hot Encoded category fields including room_type, property_type, neighborhood and host_response_time.

## Results <a name=results></a>

The results of the analysis can be found on my blog post [here](https://medium.com/@bentyesu05/how-should-you-price-your-airbnb-in-seattle-5835190d0eb9)
