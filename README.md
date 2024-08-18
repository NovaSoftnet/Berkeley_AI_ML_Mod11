# Project Documentation

## Introduction

This is a Practical Application for the Professional Certification in Machine Learning and Artificial Intelligence program.

A dataset from kaggle was used. The original dataset contained information on 3 million used cars sales but for this purpose the dataset was limited to the information on 426K cars.

## Objective

The goal is to understand what factors make a car more or less expensive. As a result of the analysis, clear recommendations should be provided to the client ( a used car dealership ) as to what consumers value in a used car.

## Procedure

The CRISP-DM model was thoroughly followed:

1. Business Understanding

* The objective is to identify how the different features of a used car affect the market price to support a car´s dealer business.
* Since the dependent variable is continuous, meaning the price value can be any number, this is considered a Regression analysis
* This analysis use Supervised learning due that we have labels assigned to specifics instances of dependent variables.
* The goal of this exercise is  to maximize the price and support the go to market and pricing strategy.

2. Data Understanding

* Every feature (column) in the dataset was carefully evaluated for adequacy and correctness
* Explored data set to define categorical and numerical features
* Features were classified as mandatory, desirable, inadequate or irrelevant
* A final subset of features was defined for modeling
 
3. Data Preparation

* Removed unselected features
* Executed featured engineering
* Removed incomplete indexes for some features 
* Transformed data accordingly using:
  * OneHotEncoding
  * Logarithm Base 10
  * CardinalEncoding
  * Scaling

4. Modeling

* The following models were used:
  * Linear Regression
  * Ridge Regression
  * Lasso Regression
* Created Pipelines to include Polynomial Feature Engineering preprocessing
* Performed Grid Search for hyperparameter tuning
* Performed Permutation Feature Importance with each model
* Performed Recursive Feature Elimination and Sequential Feature Selection for Linear and Ridge Regression

5. Evaluation

* Model performance was evaluated and compared between modules using:
  * Root Mean Square Error
  * Mean Absolute Error
* Identified best performing model and its hyperparameters
* Elaborated on findings from best model to create final business conclusions

6. Deployment

* Deliver customer Pricing Strategy Report
* Provided recommendations base on those findings

## What consumers value the most in a used car ?

The following  Report is intended to support a car´s dealer Pricing Strategy.

  ### Overview
  
  The intent of this project is to analyze historic  data from used cars sales and evaluate how the different characteristics in a vehicle influence the most its sale price 
  so current inventory can be priced and offered to customers accordingly while improving their experience and make your sales force more efficient. 
  Also make the procurement of new vehicles more efficient.
  
  ### Description
  
  The sales data was procured from a public internet source (Kaggle) and it contains a 400+ historical vehicle sales records with  detailed information like:
  
  * Sale Price
  * Model Year
  * Make and Model
  * Condition
  * Engine size and Fuel Type
  * Odometer
  * Status of the Title
  * Transmission
  * VIN
  * Drivetrain
  * Size
  * Type of Vehicle
  * Color
  * Registration State
  
  The available data was analyzed, cleaned  and processed  through well known Artificial Intelligence algorithms used to identify the main factors  that influence the sale price.
  
  ### Conclusions on most valued features
  
  After thorough simulation and careful evaluation of the modeling process, the following characteristics were found to have a  critical weight on the sale price:
  
  * Age
  * Odometer
  * Type
  * Condition
  
  However other characteristics also have considerable influence:
  
  * Title
  * Fuel Type
  * Transmission
  * Brand
  
  ### Recommendations
  
  Based on these findings, the following recommendations may help improve inventory management, customer experience and sales efficiency:
  
  * Newer vehicles tend to sales faster, occasionally classic, old sport or customized vehicles are exceptions when we talk about good sales.
  * Vehicules with Low milage and  in excelllent condition are also a good buy for customers and they are willing to pay more.
  * Pickups, trucks in good condition also have higher sale prices
  * Single owner or owners with no family or pets are highly valued for resale
  * Title status is also important for the sale.  

  ### Additional 
  
  further work should be done with propper domain knowledge to gain further insight and more detailed and valued recommendations.
