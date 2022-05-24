# Mobile-Price-Range-Prediction
Problem Statement
There are many things we consider before buying a mobile as we used our mobile for various purpose like connecting with our family & Office Colleagues, playing games ,taking a photos to keep our memory alive. So this such specifications such as RAM, internal memory ,Wi-Fi , 3G/4G connectivity etc. plays important role to buy a mobile. To analysis of this important factor from time to time and come up with the best setoff specifications and price ranges so that people will buy the mobile. Hence through the various ML modules we will help the company to estimate the price of mobiles according to feature so the maximum amount of sell will be possible.

Data Description
We have been provided with the dataset containing the 2000 rows and 21 features

• Battery power - Total energy a battery can store in one time measured in mAh

• Blue - Has Bluetooth or not

• Clock_speed -speed at which microprocessor executes instructions

• Dual_sim - Has dual sim support or not

• Fc - Front Camera mega pixels

• Four_g - Has 4G or not

• Int_memory - Internal Memory in Gigabytes

• M_dep - Mobile Depth in cm

• Mobile_wt - Weight of mobile phone

• N_cores - Number of cores of processor

• Pc - Primary Camera mega pixels

• Px_height - Pixel Resolution Height

• Px_width - Pixel Resolution Width

• Ram - Random Access Memory in Mega Bytes

• Sc_h - Screen Height of mobile in cm

• Sc_w - Screen Width of mobile in cm

• Talk_time - longest time that a single battery charge will last when you are

• Three_g - Has 3G or not

• Touch_screen - Has touch screen or not

• Wifi - Has wifi or not

• Price_range - This is the target variable with value of 0(low cost), 1(medium cost),2(high cost) and 3(very high cost).

Data Pipeline
Data Processing
Understanding and cleaning the data

Data Exploration
Analyse the data through visualization

Model Performed
• KNN

• Random Forest

• Gradient Boosting Classifier

• XGBClassifier

• Logistic Regression

Conclusion
Ram , Battery_power features were found to be the most relevant features for predicting price range of mobiles and dropping negative correlation features which are clock speed , mobile_wt , touch_screen.

Kneighbors and Xgboost are given best accuracy score 93% test ,95% train and 91% train , 88% test respectively and roc_auc score for kneighbors is 99%.

Tuning the hyperparameters by GridSearchCV on kneighbors but not getting much difference in results but the best parameters n_neighbors for train and test are 11 and 17.

So we conclude that kneighbors classifier is giving the best results for these dataset.

So we can say that in the price range prediction as the ram and battery_power increases the price range will increase for sure.
