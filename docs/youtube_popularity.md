## Popularity of Youtube Cooking Videos Prediction

**Project description:** We focused our project on cooking videos specifically as we wanted to avoid highly polarizing topics, to make it more likely that the popularity of a video is based on the content not the subject. We used the youtube api and youtube-dl to gather the data, a CNN to transform the thumbnail into a numeric feature, and used PCA to transform the vectorized texts into informative numeric features. Finally we used developed a metric that was a PCA transform of a videos likes, favorites, and views. One of the key difficulties was splitting the datasets to ensure that there was no leakage. To do this the CNN was trained on a separate dataset that was not used to train the final model.<br>

---
### Figure 1: Training Results of the CNN
The CNN train and validate mean squared error durrign training on the video thumbnails.<br>
<img src="images/CNN_training.png?raw=true">
<br>

[CNN Model Definition](https://github.com/corbinscahalan/SIADS699-capstone-project/blob/main/cnn_model.py) | [CNN Model Training](https://github.com/corbinscahalan/SIADS699-capstone-project/blob/main/cnn_train_distributed_strategy.py) | [CNN Model testing](https://github.com/corbinscahalan/SIADS699-capstone-project/blob/main/cnn_on_test_data.ipynb)

---

### Figure 2: Feature Importance
Many of the fetures in this plot are engeneered from the existing data, and the full description of each feature can be seen in Table B1 of Appendix B in our report.
<img src="images/popularity_feature_importance.png?raw=true">


---

### Figure 3: Linear Regression Base Model
The output of a base linear regression model on the test dataset. We can see that there are two outliers sevearly skewing the results.
<img src="images/popularity_lin_regression.png?raw=true">

---

### Figure 4: Ensemble Stacking Regressor
The stacking regressor on the test dataset, performed significantly better than the base linear regression model.
<img src="images/popularity_stacking.png?raw=true">

---

[Final Modeling Training and Analysis](https://github.com/corbinscahalan/SIADS699-capstone-project/blob/main/Final_model.ipynb) | 
[Final Dataset Construction](https://github.com/corbinscahalan/SIADS699-capstone-project/blob/main/construct_final_dataset.ipynb) | 
[Full Report](https://medium.com/@team_popular/predicting-youtube-cooking-video-popularity-a5b841732e2d)