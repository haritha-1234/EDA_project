# EDA on King County Housing Data

# Overview

Welcome to an Exploratory Data Analysis on the housing sales data in King County, USA. The aim of this EDA is to do a detailed analysis and give some recommendations and insights to a stakeholder who can be a buyer or seller according to his interest in a house in King County. More details on the stakeholder that I choose will be given below so that you can start the analysis keeping that info in mind. 
## Data Structure

This data contains the details of houses in King County, USA. The features of houses such as size, number of bedrooms, bathrooms, price, year of built and so on. See below: <br>
- id - unique identified for a house
- dateDate - house was sold
- pricePrice - is prediction target
- bedroomsNumber - # of bedrooms
- bathroomsNumber - # of bathrooms
- sqft_livingsquare - footage of the home
- sqft_lotsquare - footage of the lot
- floorsTotal - floors (levels) in house
- waterfront - House which has a view to a waterfront
- view - Has been viewed
- condition - How good the condition is ( Overall )
- grade - overall grade given to the housing unit, based on King County grading system
- sqft_above - square footage of house apart from basement
- sqft_basement - square footage of the basement
- yr_built - Built Year
- yr_renovated - Year when house was renovated
- zipcode - zip
- lat - Latitude coordinate
- long - Longitude coordinate
- sqft_living15 - The square footage of interior housing living space for the nearest 15 neighbors
- sqft_lot15 - The square footage of the land lots of the nearest 15 neighbors 
## Stakeholder 
Jacob Phillips : Buyer
<br>
Characteristics:
- Unlimited budget
- 4+ bathrooms or smaller house nearby 
- Big lot (tennis court & pool), golf, historic, no waterfront
<br>

My stakeholder wants to buy a house in Seattle, which has 4+ number of bathrooms and is away from water front. So my inspiration was to look for a house whose size is larger than the mean size of the total houses given, somewhere inside the County where there are small number of neighborhood. 

At the end, I want to recommend a location with a house to my stakeholder which satisfies his requirements! Full EDA is given in [EDA.ipynb](./EDA.ipynb) 
## Motivation
- Are the houses built in later 90's has more features, and hence more expensive? If not, why?

- How many houses are there with more than 4+ bathrooms?

- Where are these houses located? near or far from waterfront? 

# Settings
## Requirements
Python version:
- pyenv
- python==3.9.4

## Setup
Setting up the virtual environment.

For this purpose you use following commands:

```bash
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```

## Unit testing (Optional)

If you write python scripts for your data processing methods, you can also write unit tests. In order to run the tests execute in terminal:

```bash
pytest
```

This command will execute all the functions in your project that start with the word **test**.
