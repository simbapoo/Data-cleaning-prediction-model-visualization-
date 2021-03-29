# Data-cleaning-prediction-model-visualization
We have some dataset from Krisha.kz, we need to clean this dataset

1.First of all to work with cleaned data we need to see the outliners in column “price” let’s see the max value of “price”
and the let’s give a limit for “price”
anyway it will be hard to work with “price”, that’s why decided divide “price” to 1000
In this plot described frequency of district. 

Where 

1=Бостандыкский р-н

2=Медеуский р-н

3= Алмалинский р-н

4= Ауэзовский р-н

5= Жетысуский р-н

6= Алатауский р-н

7= Турксибский р-н

8= Наурызбайский р-н

and we se that Бостандыкский р-н many apartments for sales

2. Let’s take three columns “price”, “area” and “district” from our dataset and see what we can infer by plotting to scatter plot 
between price vs area and district vs price
  
  Now, let’s plot Pair Plots for the three columns we used in plotting Scatter plots. We’ll use the seaborn
 library for plotting Pair Plots.
 
Variables:district,area,year helps to predict apartment prices

 3. Our regression consist:rooms,floor coef, year, area
first of all we run regression with 5 parameters, and our score 0.7993% then we remove last parameter and we have 0.7955%
after that we delete floor_coef and return year out score 0.7992% after that we delete rooms and return coef our score 0.7960%
after that we delete area and return rooms our score 0.5815%
Our final decision area have more impact on price than other parameters
5.New predictor district help us to distribute prices of houses of Almaty
We take this parameters from street column
Next predictor extra features predictors which define extra features of house like:internet,gas, school, security, etc...
Next predictor the quantity of pictures increase addiction for apartment sell announcement
