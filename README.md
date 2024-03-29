# Predicting-Concrete-Strength-using-Neural-Networks
## Summary
This work is a derivative of the "From Mix to Model" project, I wanted to compare the results obtained in the laboratory with the ones predicted by the model. The results showed that the other project's model indeed worked but it also stablished the importance of the security factor in any mix design.

## Data Used

The data is the same as the other project, the change I made was the variables. Now the output data is just "Concrete Strength at 28 days"
### Input Data
- Cement Brand
- Specific Weight of Cement
- Dry Specific Weight of Fine Aggregate
- Fineness Module of Fine Aggregate
- Dry Specific Weight of Coarse Aggregate
- Fineness Module of Coarse Aggregate
- Nominal Maximum Size
- Slump
- Cement Weight
- Fine Aggregate Weight
- Coarse Aggregate Weight
- Water Weight
### Output Data
- Concrete Strength at 28 days

## Technologies Used 
- TensorFlow
- Pandas
- Keras
- Scikit-learn
- Matplotlib

## Results and Conclusions

I deciced to test this model using the designs from the other project. in order to find out how the model works along with the security factor needed for any design.

Cement Brand | Specific Weight of Cement | Dry Specific Weight of fine Aggregate | Fineness module of Fine Aggregate | Dry Specific Weight of coarse Aggregate | Fineness module of Coarse Aggregate | Nominal Maximum Size | Slump | Cement Weight | Fine Aggregate Weight | Coarse Aggregate Weight | Water Weight 
------------- | -------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ----------- | ---------- | -------
3 |2850 | 2596.42459 | 2.42 | 2715.18145 | 6.17 | 0.5 |  4 | 408.52 | 833.97 | 769.34 | 232.29
3 |2850 | 2596.42459 | 2.42 | 2715.18145 | 6.17 | 0.5 |  4 | 436.17 | 820.14 | 749.34 | 235.80
3 |2850 | 2596.42459 | 2.42 | 2715.18145 | 6.17 | 0.5 |  4 | 480.01 | 780.96 | 739.33 | 239.42 
3 |2850 | 2445.77632 | 3.18 | 2500.30754 | 6.93 | 0.75 |  4 | 351.73 | 650.77 | 1009.54 | 198.08
3 |2850 | 2445.77632 | 3.18 | 2500.30754 | 6.93 | 0.75 |  4 | 391.54 | 623.67 | 988.33 | 200.77
3 |2850 | 2445.77632 | 3.18 | 2500.30754 | 6.93 | 0.75 |  4 | 440.55 | 587.81 | 968.45 | 205.82

This is the output data: 

Design Name | Concrete Strength at 28 days 
---------- | -----------
B-175 | 251.300
B-210 | 281.812
B-280 | 333.978
L-175 | 250.065
L-210 | 297.479
L-280 | 351.608

### FIRST CONCLUSION

Look at the following table of the previous project's Tested Results  

Design Name | Concrete Strength at 28 days 
---------- | -----------
B-175 | 185.83
B-210 | 211.53
B-280 | 236
L-175 | 192.27
L-210 | 215.43
L-280 | 246.33

Upon observation, the predicted results don't align with the tested ones. However, if you subtract the security factor (70 for 175, 84 for 210 and 280) from the predicted results, both tested and predicted results become similar. The primary conclusion drawn from this predictive project is the necessity of a comprehensive database encompassing various concrete designs for accurate strength prediction. Nonetheless, the development of a method for concrete design using ANN is a feasible with a well-balanced database for each resistance
