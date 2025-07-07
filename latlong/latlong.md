Based on attempts at region id, the model for lat long prediction had the following features: 
- **Ensemble model** combining the results of ConvNeXt and Swin. The ensemble results were weighted as a function of their MSE on the val set. The model combined performed was consistently better than both models, implying that both models were learning orthogonally. 
- **Using Region ID** for predicting the angle in the test set. The model predicts the region id and then uses that as a one-hot embedded vector in order to produce results. 
 