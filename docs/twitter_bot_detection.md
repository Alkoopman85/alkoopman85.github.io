## Twitter Bot Detection

**Project description:** In this project we creted two datasets, one was made up of only the tweets for each user concatenated together, we then used a neural net on those tweets in TF-IDF format to calssify an account as a bot or a human. The output of this was then included in the data for an ensemble model which did the final prediction. This project included extensive feature engeneering and extraction to create an array of features for the final model (a full list of these can be seen in the final report). Note that this was before verified status became fee based.<br>

---

### Figure 1: Imporuty Based Feature Importance
<img src="images/twitter_users_feature_importance.png?raw=true">

---
### Figure 2: Umap Projection of The Twitter Users (human: 0 bot: 1)
<img src="images/twitter_users_umap.png?raw=true">

---
### Figure 3: Basic Logistic Regression
<img src="images/twitter_bot_logistic_regression.png?raw=true">

---
### Figure 4: Ensemble Voting Classifier
<img src="images/twitter_bot_voting_classifier.png?raw=true">

---
### Figure 5: Ensemble Stacking Classifier
<img src="images/twitter_bot_stacking_classifier.png?raw=true">

---
[Full Report]("/pdfs/Twitter Bot Detection SIADS 694_695 Team Project Report.pdf") | [Final Modeling Notebook](https://github.com/MarlonShakespeare/Milestone-2/blob/main/final_supervised_model.ipynb)