# Mobile-price-range-prediction

# PROBLEM STATEMENT:

In the competitive mobile phone market companies want to understand sales data of mobile phones and factors which drive the prices. The objective is to find out some relation between features of a mobile phone(eg:- RAM, Internal Memory, etc) and its selling price. In this problem, we do not have to predict the actual price but a price range indicating how high the price is.

**Data Description -**

*   **Battery_power** - Total energy a battery can store in one time measured in mAh
*   **Blue** - Has bluetooth or not
*   **Clock_speed** - speed at which microprocessor executes instructions
*   **Dual_sim** - Has dual sim support or not
*   **Fc** - Front Camera mega pixels
*   **Four_g** - Has 4G or not
*   **Int_memory** - Internal Memory in Gigabytes
*   **M_dep** - Mobile Depth in cm
*   **Mobile_wt** - Weight of mobile phone
*   **N_cores** - Number of cores of processor
*   **Pc** - Primary Camera mega pixels
*   **Px_height** - Pixel Resolution Height
*   **Px_width** - Pixel Resolution Width
*   **Ram** - Random Access Memory in Mega
*   **Touch_screen** - Has touch screen or not
*   **Wifi** - Has wifi or not
*   **Sc_h** - Screen Height of mobile in cm
*   **Sc_w** - Screen Width of mobile in cm
*   **Talk_time** - longest time that a single battery charge will last when you are
*   **Three_g** - Has 3G or not
*   **Price_range** - This is the target variable with value of 0(low cost), 1(medium cost), 2(high cost) and 3(very high cost).

# Steps involved:

**Exploratory Data Analysis** 

Exploratory data analysis is an statistical way of understanding the data which is usually done in a visual way. The graphs plotted in exploratory data analysis are for better understanding of data to the analyst. 
After loading the dataset we performed this method by comparing our target variable with other independent variables. This process helped us figuring out various aspects and relationships among the target and the independent variables. It gave us a better idea of which feature behaves in which manner compared to the target variable.

**Null values Treatment**

After the data is loaded , The missing data is checked using is.na() or isnul() function . The output depicted that there was many  missing values in our dataset.

 **Feature Engineering**
 
To make the data tenable for understanding and further analysis , the data set was analyzed for identifiable statistical trends and patterns. 

**Standardization of features**

Our main motive through this step was to scale our data into a uniform format that would allow us to utilize the data in a better way while performing fitting and applying different algorithms to it. 
The basic goal was to enforce a level of consistency or uniformity to certain practices or operations within the selected environment.

**Evaluation of models**

For modelling we tried various  algorithms like:

Linear Regression

KNN

Logistic Regression

Decision tree

Random forest.

SVM 

# Conclusion:

We Started with Data understanding, data wrangling, basic EDA where we
found the relationships, trends between price range and other independent
variables.

We selected the best features for predictive modeling by using K best feature
selection method using Chi square statistic.

Implemented various classification algorithms, out of which the SVM(Support
vector machine) algorithm gave the best performance with 94% train accuracy
and 90 % test accuracy.

XG boost is the second best good model which gave good performance 98%
train accuracy and 89% test accuracy score.
KNN gave very worst model performance.

We checked for the feature importance's of each model. RAM, Battery
Power, Px_height and px_width,Screen size,mobile weight contributed the
most while predicting the price range.


