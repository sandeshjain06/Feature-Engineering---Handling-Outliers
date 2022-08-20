# Feature-Engineering - Handling-Outliers


Techniques for Outlier Detection and Removal


1. Z-Score Treatment        :    x-mean / std 
2. IQR based filtering      :    75percentile - 25percentile 
3. Percentile
4. Winsorization Technique 


If Data Distribution is in Linear Form
        
        
          Finding Outliers or Replacing Outliers using : Upper/Lower bound (2) , Z-score (1)

          1)Upper bound :  x.mean() + 3* x.std() , Lower bound : x.mean() - 3* x.std()

          2)Z-Score :   x-mean / std 
          
          It will convert all the values in range (3,-3) , any values which are lying outside this can be considered as outliers.



If Data Distribution is in Non-Linear Form 

        Finding Outliers or Replacing Outliers using : IQR  (2)
        1) IQR = 75percentile - 25percentile  
        2) Upper bound = 75percentile + 1.5 IQR  
        3) Lower bound = 25percentile - 1.5IQR



Winsorization
 
        Explicitly we can define the Upperlimit and lowerlimit .

        Upper limit and lower limit diff should be same such as 99 / 1 , 98/2 ,97/3,96/4 .


