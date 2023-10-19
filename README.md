# Walmart-Sales-Forecasting
![image](https://github.com/this1shung/Walmart-Sales-Forecasting/assets/126255184/d23f85af-a23b-43c8-9846-5ae2be866214)
### Infomation about this project : 
 - This project is a recruiting competion from walmart : Walmart is a multinational retail corporation based in the United States. It is one of the largest and most well-known retail chains in the world. Founded in 1962 by Sam Walton, Walmart operates a variety of retail formats, including supercenters, discount stores, warehouse clubs, and e-commerce platforms. 

# 1.Problem definition 

 - Regression problem (predicting the Weekly_Sales values of 45 walmart store using the Weekly_Sales from the previous year)

# 2.Data 

 - The data for this project is from kaggle: https://www.kaggle.com/competitions/walmart-recruiting-store-sales-forecasting/data
 
 - We got about 4 data set for this project

   + stores.csv : This file contains anonymized information about the 45 stores, indicating the type and size of store

   + train.csv : This is the historical training data, which covers to 2010-02-05 to 2012-11-01. Within this file you will find the following fields

          *  Store - the store number

          *  Dept - the department number

          *  Date - the week

          *  Weekly_Sales -  sales for the given department in the given store

          *  IsHoliday - whether the week is a special holiday week

   + test.csv :  This file is identical to train.csv, except we have withheld the weekly sales. You must predict the sales for each triplet of store, department, and date in this file.
  
   + features.csv : This file contains additional data related to the store, department, and regional activity for the given dates. It contains the following fields:

          *  Store - the store number

          *  Temperature - average temperature in the region

          *  Fuel_Price - cost of fuel in the region

          *  MarkDown1-5 - anonymized data related to promotional markdowns that Walmart is running. MarkDown data is only available after Nov 2011, and is not available for all stores all the time. Any missing 
             value is marked with an NA.

          *  CPI - the consumer price index

          *  Unemployment - the unemployment rate

          *  IsHoliday - whether the week is a special holiday week

     + For convenience, the four holidays fall within the following weeks in the dataset (not all holidays are in the data) so I have to added another columns to specific the holiday 

           *Super Bowl: 12-Feb-10, 11-Feb-11, 10-Feb-12, 8-Feb-13

           *Labor Day: 10-Sep-10, 9-Sep-11, 7-Sep-12, 6-Sep-13

           *Thanksgiving: 26-Nov-10, 25-Nov-11, 23-Nov-12, 29-Nov-13

           *Christmas: 31-Dec-10, 30-Dec-11, 28-Dec-12, 27-Dec-13
      + Because the data this time is split into four files, I used the pd.merge method to combine them together in order to leverage various attributes to support the performance of the ML model


# 3. Evaluation metrics  
  
  - This competition is evaluated on the weighted mean absolute error (WMAE):
    ![image](https://github.com/this1shung/Walmart-Sales-Forecasting/assets/126255184/398187e3-2607-4922-a9d1-a8802f5e518d)
  
  - I have build the function to evaluate the model base on the require metrics from

# 4. Model
  
  - After several try with different model I end up using RandomforestRegressor

  - In addition, to improve the model's performance, I have taken steps to normalize categorical data and removed less-contributing attributes for the model.

# Final :

- This is the 1st time i try to submit my work to kaggle. After several submission file with huge score like, 25k, 26k, i try do my work in another way like : change the way i merge the dataset, sort the data, remove less contributing attributes,......

- This is my final score :
  ![image](https://github.com/this1shung/Walmart-Sales-Forecasting/assets/126255184/ef82aba3-ec95-44f8-a53b-2d1b7f4684e0)

# Some picture about my project: 
![image](https://github.com/this1shung/Walmart-Sales-Forecasting/assets/126255184/66315393-e81f-44f9-8529-22ac0bca71e9)
![image](https://github.com/this1shung/Walmart-Sales-Forecasting/assets/126255184/5f5f817e-42a5-47e6-969e-9f9669ad41eb)
![image](https://github.com/this1shung/Walmart-Sales-Forecasting/assets/126255184/4e4cd805-a7a3-48ac-ad5a-d3abb97f2078)
![image](https://github.com/this1shung/Walmart-Sales-Forecasting/assets/126255184/daec502f-ef5b-4521-83dd-26b05f49761a)
![image](https://github.com/this1shung/Walmart-Sales-Forecasting/assets/126255184/ccb0b10c-8468-4121-9e6c-a58438c1a8f3)

Thank you for reading my project details if you have any idea to improve this project feel free to contact me, it will help me a lot. 

Wishing you a great day!

## 📫 How to reach me: <a href="https://hungmondaypkm@gmail.com" target="blank"><img align="center" src="https://img.icons8.com/color/48/000000/gmail--v2.png" alt="hungmondaypkm@gmail.com" height="30" width="40" /></a><a href="https://www.facebook.com/profile.php?id=100009216758210" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/facebook.svg" alt="1" height="30" width="40" /></a><a href="https://twitter.com/gnuhmonday" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/twitter.svg" alt="1" height="30" width="40" /></a><a href="https://www.linkedin.com/in/quang-h%C6%B0ng-l%C3%AA-989610293/" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="1" height="30" width="40" /></a>






    
  
     




