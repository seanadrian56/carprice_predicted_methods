# carprice_predicted_methods
The objective of this notebook is to decide which indicators/variables can be use as the predictor of car price in the future.

## Loading the data
First, let's load the data into our notebook.

![image](https://user-images.githubusercontent.com/118429391/208048245-8c6bf0a6-53e3-4f60-9ef0-2a715957d61a.png)
There are some indicators that has some missing/unknown values. Before going to alayze it, let's change and complete all the missing value and correct the data format.

## Data Wraggling 

![image](https://user-images.githubusercontent.com/118429391/208048769-43ea1526-7a8c-45bc-850e-784374c11580.png)
After we fullfill the missing value, let's convert and normalize some of our data into a proper one. 

![image](https://user-images.githubusercontent.com/118429391/208050189-c2318392-1d01-4e27-9846-82c994a0854f.png)

In this case, we convert city-mpg and highway-mpg to city-L/100km and highway-L/100Km. We also normalize "length", "width" and "height" columns. We also categorize horse power columns and indicate dummy variables for fuel type and aspiration. After all set, we can analyze the data using some of data visualization tools. 

## Data Visualization

### Engine size and price

![image](https://user-images.githubusercontent.com/118429391/208051148-497d1b5e-e1ae-40bd-9c7a-2361314c9d2f.png)

### Highway-L/100Km and price

![image](https://user-images.githubusercontent.com/118429391/208051292-18dec150-7023-4e3c-a76e-6b5ed269cdb1.png)

### Peak-rpm and price

![image](https://user-images.githubusercontent.com/118429391/208051434-6f7c05f5-559b-4546-ac43-e0c62b4e687b.png)

### Stroke and price

![image](https://user-images.githubusercontent.com/118429391/208051765-2d86c28c-bb0a-4a0d-a51f-6ae9e0527b3b.png)

### Body Style and price

![image](https://user-images.githubusercontent.com/118429391/208052087-a1ab727e-0cf9-4e6a-874a-8ded9e3db652.png)

### Engine location and price

![image](https://user-images.githubusercontent.com/118429391/208052443-a7852f9f-f1ab-464e-90a4-8d1f974107c9.png)

### Drive wheels and price

![image](https://user-images.githubusercontent.com/118429391/208052553-7170487d-1746-49a0-b6e5-7f8eba65aa88.png)

### Body style and price

![image](https://user-images.githubusercontent.com/118429391/208052678-09dfed72-c1cd-4c87-aecb-ce3f2242c1c4.png)

## Correlation and Causation

### Wheelbase vs price
The Pearson Correlation coefficient is 0.584 with a P-Value of 8.076e-20
### Horse power vs price
The Pearson Correlation coefficient is 0.809 with a P-Value of 6.273e-48
### Length vs price
The Pearson Correlation coefficient is 0.690 with a P-Value of 8.016e-30
### Width vs price
The Pearson Correlation coefficient is 0.751 with a P-Value of 9.200e-38
### Curb-weight vs price
The Pearson Correlation coefficient is 0.834 with a P-Value of 2.189e-53
### Engine size vs price
The Pearson Correlation coefficient is 0.872 with a P-Value of 9.265e-64
### Bore vs price
The Pearson Correlation coefficient is 0.543 with a P-Value of 8.049e-17
### City-L/100 Km vs price
The Pearson Correlation coefficient is 0.789 with a P-Value of 3.903e-44
### Highway-L/100Km vs price
The Pearson Correlation coefficient is 0.801 with a P-Value of 3.086e-46

## Conclution
We now have a better idea of what our data looks like and which variables are important to take into account when predicting the car price. We have narrowed it down to the following variables:

Continuous numerical variables:
Length, Width, Curb-weight, Engine-size, Horsepower, City-mpg, Highway-mpg, Wheel-base, Bore,

Categorical variables:
Drive-wheels
