# AI-Model-for-Predicting-House-price
Predicting apartment, house price using XGBoost, MLP methods. 
MLP structure:
![image](https://user-images.githubusercontent.com/65017142/223495779-470b2d9a-8dc2-4053-8089-852a2246927f.png)

XGBoost structure:
![image](https://user-images.githubusercontent.com/65017142/223495876-88ecd038-d70b-43b7-88c6-fe6e96365aa8.png)

Variables:
  -City, country, district
  -Dedicated area
  -Contract year and month
  -Transaction amount
  -Floor level
  -Year of construction
  -Whithin 600m of 
    -Starbucks
    -Subway Station
    -Schools and daycare centers
    -Supermarkets, big stores
    -Hospital
    -Park
Some of Data Correlation graphs:
Transaction volume, Year of construction:
![image](https://user-images.githubusercontent.com/65017142/223498007-b2384a68-d7b3-4bbc-a040-9e5bbc08403b.png)

Transaction amount, Floor level:
![image](https://user-images.githubusercontent.com/65017142/223498063-bf977d5c-2925-4545-87d4-b8b9a2d8faf8.png)

Transaction amount, Subway station:
![image](https://user-images.githubusercontent.com/65017142/223498329-38561035-cf81-464e-b5fb-511b5613b0c7.png)

By these graphs we can know how much these variables can affect transaction volume(price of the apartment)

RMSE value of the test batch(epoch=1000, learning rate=0.001 mini-batch=64):

![image](https://user-images.githubusercontent.com/65017142/223503240-eba2001b-ac6b-4609-b096-b15de40e72bc.png)



To run you have to install:
streamlit==1.10.0
sklearn==0.0
matplotlib==3.5.1
numpy==1.22.3
pandas==1.4.2
xgboost==1.6.1
openpyxl==3.0.9
