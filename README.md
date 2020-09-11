# Microsoft Azure Machine Learning Scholarship Showcase Project  

[image1]: ./images/cleanDfVisual.png    
[image2]: ./images/heatmap.png 
[image3]: ./images/wightedPriceUncleanData.png 
[image4]: ./images/bidirectionalLSTMLoss.png
[image5]: ./images/BidirectionalLSTMpredictVStrue.png
[image6]: ./images/RMSE.png
[image7]: ./images/mutil_feature_train_loss.png
[image8]: ./images/predictvsTrueMulti.png
[image9]: ./images/RMSEMulti.png
[image10]: ./images/scatterplotActualVSPredict.png
[image11]: ./images/MultiScatterPlot.png


| Name | Slack Name |
| ------------------------- | ------------------------- |
| [Hsin Wen Chang](https://github.com/Polarbeargo) | Hsin-Wen Chang |

### Forecasting Time Series Cryptocurrency Prices Using Machine Learning  
Forecasting model of cryptocurrencies prices using machine learning approach with three year data 

### Clean & Visualize data with Plotly
Original Data Frame With Plotly       | Cleaned Data Frame With Plotly
:-------------------------:|:-------------------------:
![][image3]                | ![][image1] |  

### Data Correlation  
![][image2]

### Scaling Data  

* Using MinMax normalize to fit feature Weighted Price  then transforming it so that the values fit within a range or scale between 0–1.[MinMaxScaler](https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.MinMaxScaler.html)

### Model Architecture Summary  
```
Model: "sequential_18"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
bidirectional_15 (Bidirectio (None, 200)               81600     
_________________________________________________________________
dense_17 (Dense)             (None, 1)                 201       
=================================================================
Total params: 81,801
Trainable params: 81,801
Non-trainable params: 0
_________________________________________________________________
None  
```
### Results  

Training Loss (single feature)|  Training Loss (multi feature)|
:-------------------------:|:-------------------------:|
![][image4]                |  ![][image7]              |

Predict VS True (single feature)| Predict VS True (multi feature)|   
:-------------------------:|:-------------------------:|
![][image5]                | ![][image8]                | 

RMSE (single feature)      |RMSE (multi feature)  
:-------------------------:|:-------------------------:|
![][image6]                |![][image9]

![][image11]


### References    
* [Microsoft Azure Scholarship 
Project Showcase Challenge Guideline](https://docs.google.com/document/d/1p0rplg0ZrIFfBabY1WyhyVOxjVjxMORC3koV00rscAI/edit#heading=h.dauwh6uej7if)  
* [Forecasting Cryptocurrency Prices Time Series Using
Machine Learning](http://ceur-ws.org/Vol-2422/paper26.pdf)  
* [Developing and Deploying a Churn Prediction Model with Azure Machine Learning Services](https://devblogs.microsoft.com/cse/2019/01/10/develop-and-deploy-a-hybrid-multi-input-churn-prediction-model-with-azure-machine-learning-services/)
* [MinMaxScaler](https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.MinMaxScaler.html)
