# Store-Sales-Forecast-with-SARIMA
- [Project Goal](#Project-Goal)
- [File Descriptions](#File-Descriptions)
- [Instructions](#How-To-Run-This-Project)
- [Exploratory Data Analysis (EDA)](#EDA)
- [SARIMA Model](#Model)
- [Licensing, Authors, Acknowledgements](#License)

## Project Goal <a name="Project-Goal"></a>
The goal of this project is to forecast the sales of a superstore over a 10-month period using the SARIMA model to forecast time series data.

**Background:** The given dataset contained sales of a superstore from 2015 to 2018. The store's products are technology, furniture, and office supplies.

## File Description <a name="File-Descriptions"></a>
There are 2 files in this repository. <br>
A jupyter notebook `.ipynb` entails the analysis. <br>
A README.md file as a brief look at this repository.

## Instructions <a name="How-To-Run-This-Project"></a>
* Execute the codes in this notebook and follow along with the insights to understand the decisions made throughout the process.
* This project can also be found in my Kaggle [post](https://www.kaggle.com/code/azeotrope/store-sales-forecasting-with-sarima)

## Exploratory Data Analysis (EDA) <a name="EDA"></a>

![10_states](img/state.png)<br>
Figure 1. Top 10 states where the store's sales are from.

Most of the store's sales are from California and New York states. Sales from these 2 states seem to make up 50% of the store's sales, followed by Texas, Washington, and Pennsylvania. 

![10_cities](img/city.png)<br>
Figure 2. Top 10 cities generate sales for the store.

The top 10 cities generating sales are corresponding to the observed top states above. Top the charts are New York City (NY), Los Angeles (CA), Seattle, San Francisco (CA), and Philadelphia. 

![customers](img/cust_seg.png)<br>
Figure 3. Portions of customers purchase from the superstore.

The main customers of the superstore are classified as general consumer, corporate, and home office. The general consumer made up 50.8% of the purchases and corporate made up 30.4%.

![products](img/product_cat.png)<br>
Figure 4. Sales distributions from the three product categories: technology, furniture, and office supplies.

The superstore product categories are technology, furniture, and office supplies. Overall, the sales are equally distributed amongst the 3 categories. 

## SARIMA Model <a name="Model"></a>
The model is first built on the train set, then predicts the sales on the test set. 
The mean forecast error of this model is 132.72 which indicates **under-forecasting**. 

![SARIMA](img/SARIMA_model.png)<br>
Figure 5. Model's prediction on the given dataset and its forecast for the next 10 months.

The model is then fit and trained on the whole original dataset, then forecast the sales for the next 10 months. 
The model predicts a sales revenue more conservatively in contrast with the actual sales that is quite fluctuated.

## Licensing, Authors, Acknowledgements <a name="License"></a>
* The data set, licensing, and other descriptive information are described here [Kaggle](https://www.kaggle.com/datasets/rohitsahoo/sales-forecasting)
