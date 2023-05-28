# Project Title
Module-21-Neural-Network

## Overview of the Analysis
The purpose of this analysis was to determine which appllicant has made us of the funding provided by he nonprofit foundation called Alphabet Soup. <br>


## Results
The data consist of: <br>
* EIN and NAME—Identification columns
* APPLICATION_TYPE—Alphabet Soup application type
* AFFILIATION—Affiliated sector of industry
* CLASSIFICATION—Government organization classification
* USE_CASE—Use case for funding
* ORGANIZATION—Organization type
* STATUS—Active status
* INCOME_AMT—Income classification
* SPECIAL_CONSIDERATIONS—Special considerations for application
* ASK_AMT—Funding amount requested
* IS_SUCCESSFUL—Was the money used effectively

Both EIN and NAME columns had to be removed becasue they both were neither targets or features. <br>

Our target variable was the column "IS_SUCCESSFUL" <br>

Our features were: <br>
* APPLICATION_TYPE
* AFFILIATION
* CLASSIFICATION
* USE_CASE
* ORGANIZATION
* STATUS
* INCOME_AMT
* SPECIAL_CONSIDERATIONS
* ASK_AMT
* IS_SUCCESSFUL

For the original model:<br>
* Layer and neurons
    * reLU-80
    * reLU-30
    * Sigmoid-1

At 100 Epoch, this resulted in a loss of 0.5592 and accuracy of 0.7255 <br>

For the optimized model:<br>
* Layer and neurons
    * reLU-200
    * reLU-80
    * reLU-20
    * Sigmoid-4
    * Sigmoid-1

At 100 Epoch, this resulted in a loss of 0.5391 and accuracy of 0.7401 <br>

The study compared two neural network models, an optimized version and an original model. The optimized model demonstrated better performance, thanks to a series of modifications. The dataset was preprocessed by reducing the number of columns through binning, resulting in a more focused set of features for the model to learn from. Additionally, the optimized model featured an increased number of layers and neurons, aiming to capture complex patterns and relationships. However, despite these improvements, the model fell short of achieving the targeted accuracy of 0.75.

## Summary 
In summary, the optimized neural network model outperformed the original model. The enhancements included reducing column count through binning and adding more layers and neurons. While these changes improved performance, the model could not attain the desired accuracy threshold. Further investigation or adjustments may be necessary to achieve the specified accuracy goal.

## Contributing
Alan Deng

## Resources
Stack Overflow, W3school