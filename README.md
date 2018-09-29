# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Kaggle Competition - Starter

## Introduction

Welcome to your first week of work at the Disease And Treatment Agency, division of Societal Cures In Epidemiology and New Creative Engineering (DATA-SCIENCE). Time to get to work!

Due to the recent epidemic of West Nile Virus in the Windy City, we've had the Department of Public Health set up a surveillance and control system. We're hoping it will let us learn something from the mosquito population as we collect data over time. Pesticides are a necessary evil in the fight for public health and safety, not to mention expensive! We need to derive an effective plan to deploy pesticides throughout the city, and that is **exactly** where you come in!

## Dataset

The dataset, along with description, can be found here: [https://www.kaggle.com/c/predict-west-nile-virus/](https://www.kaggle.com/c/predict-west-nile-virus/).


**Project Planning**
Given previous cases of West Nile Virus, can we predict the presence of the virus for a given time, location and species in Chicago?

**EDA**

First, I will clean the data. This process will replace any missing values with the mean of the column and any values recorded as Trace will be replaced with a very small number.
I then will visualize all the data on a map of Chicago.

Following that step, I will feature engineer some relationships in the data.
Feature Engineering
Average both Weather Stations' temperatures

Using information, I have read about mosquitoes and its life cycles, I incorporate variables time lag after rainfall, wet bulb(measure of water vapor and humidity), and dew point(humidity).

Time Lag after Rain, Wet Bulb, and Dew Point- 1,3,7,14 days after

I also will factor in the duration of the day as a variable.

**Modeling**

1. The goal is of course to build a model and make predictions that the city of Chicago can use when it decides where to spray pesticides!

Models I will use:
Logistic Regression
Gradient Boosting Classifier
Random Forest Classifier
XGBoost Classifier
Support Vector Machine Classifier

I will evaluate each of these models by the area under the Receiving Operating Curve score I obtain. The higher this value, the more accurately the model identifies true positives in the data.

Possible Future Studies
What is the impact of the spray on West Nile Virus in Chicago? More specifically, what types of mosquito spray are being used? How are they being applied across the city? How effective is the spray?
