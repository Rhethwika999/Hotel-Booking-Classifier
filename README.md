# Hotel Booking Cancellation Classifier :hotel:

## Aim :mag:
To develop a classification model that predicts hotel booking cancellations, enabling hotels to proactively manage occupancy rates and enhance operational efficiency.

---

## Objectives :dart:
* Analyze historical booking data to identify patterns and key factors influencing cancellations.
* Preprocess and clean the dataset to ensure data quality and suitability for modeling.
* Implement and evaluate various machine learning algorithms to achieve optimal prediction accuracy.
* Provide actionable insights and recommendations based on model results to assist in decision-making.

---

## Built using 🛠️
* Python

---

## Dataset :bar_chart:
The dataset contains 119391 rows and 32 columns. It contains detailed booking records for a resort hotel, spanning from July 2015 to July 2016. It provides comprehensive information on various aspects of hotel bookings, including guest demographics, booking details, financial information, and reservation patterns.


### Key Features

1. **Booking Details**:
   - **Dates**: Arrival and departure dates, length of stay (1 to 31 days)
   - **Guests**: Number of adults, children, and babies per booking
   - **Meal Plans**: Types include Bed & Breakfast (BB), Half Board (HB), Full Board (FB), and Self Catering (SC)
   - **Countries of Origin**: Guests from various countries, including Portugal (PRT), Great Britain (GBR), Spain (ESP), Germany (DEU), France (FRA), Ireland (IRL), Brazil (BRA), USA, China (CN), and others

2. **Booking Status**:
   - **Statuses**: Check-Out, Canceled, No-Show, Transient
   - **Cancellation Rates**: High cancellation rates, with many reservations canceled well in advance

3. **Booking Channels**:
   - **Channels**: Online Travel Agent (TA), Offline TA/TO (Tour Operator), Direct, Corporate, Groups
   - **Market Segments**: Transient, Transient-Party, Contract, Group

4. **Financial Details**:
   - **Deposit Types**: Mostly "No Deposit," with some "Non Refund" and "Refundable"
   - **Average Daily Rate (ADR)**: Varies significantly across bookings
   - **Special Requests**: Some bookings include special requests and car parking spaces

5. **Reservation Patterns**:
   - **Lead Time**: Varies significantly, from 0 to 394 days
   - **Customer Types**: Mostly transient, with a few transient-party and contract customers
   - **Room Types**: Reserved and assigned room types vary, with some changes made to bookings

####Note : This project was completed as part of the [LearnBay](https://www.learnbay.co/) "Advanced Data Science and AI" course . The dataset used for this hands-on assessment was provided by the course instructors.
---


## Libraries and Packages Used 📦

The following Python libraries and packages were used in this project:

- **pandas**: Data manipulation and analysis.
- **numpy**: Numerical operations and array handling.
- **seaborn**: Data visualization (with `sns.set(color_codes=True)` for color styling).
- **matplotlib**: Plotting and visualization (imported `pyplot` and `Axes3D`).
- **warnings**: Handling and filtering warnings.
- **scikit-learn (sklearn)**:
  - `train_test_split`: Splitting data into training and testing sets.
  - `GridSearchCV`: Hyperparameter tuning using cross-validation.
  - `StandardScaler`: Standardizing data (scaling features).
  - `accuracy_score`: Evaluating model performance.
  - `confusion_matrix`: Generating confusion matrix for classification tasks.
  - `classification_report`: Generating classification reports.
  - `LogisticRegression`: Logistic regression model.
  - `KNeighborsClassifier`: K-nearest neighbors classification.
  - `SVC`: Support Vector Classifier.
  - `DecisionTreeClassifier`: Decision tree classification model.
  - `RandomForestClassifier`: Random forest classification model.
  - `LabelEncoder`: Label encoding for categorical variables.
  - `OneHotEncoder`: One-hot encoding for categorical features.
 
---

## Methodology 📈

In this project, we employed several statistical and machine learning techniques to analyze the hotel bookings dataset and derive meaningful insights. The following methods were used:

### 1. Correlation Analysis
- **Heatmap**: We generated a correlation heatmap to visualize the relationships between different numerical features in the dataset. This helped identify which variables are strongly correlated with each other, providing insights into potential predictors for booking cancellations and other outcomes.

### 2. Logistic Regression
- **Logistic Regression**: This technique was used to model the probability of booking cancellations. By fitting a logistic regression model, we were able to understand the impact of various features on the likelihood of a booking being canceled.

### 3. Random Forest
- **Random Forest**: We implemented a random forest classifier to predict booking cancellations. This ensemble method, which combines multiple decision trees, helped improve the accuracy and robustness of our predictions by reducing overfitting.

### 4. K-Nearest Neighbors (KNN)
- **K-Nearest Neighbors**: The KNN algorithm was used to classify bookings based on their similarity to other bookings. This method is particularly useful for understanding patterns in the data and making predictions based on the proximity of data points in the feature space.

### 5. Decision Trees
- **Decision Trees**: We utilized decision trees to model the decision-making process for booking cancellations. Decision trees provide a clear and interpretable structure for understanding how different features influence the outcome.

### Implementation Steps
1. **Data Preprocessing**: 
   - Cleaned the dataset by handling missing values and encoding categorical variables.
   - Split the dataset into training and testing sets to evaluate model performance.

2. **Exploratory Data Analysis (EDA)**:
   - Conducted EDA to understand the distribution of features and identify any anomalies or patterns.
   - Generated visualizations such as  the correlation heatmap, to aid in feature selection.

3. **Model Training and Evaluation**:
   - Trained each model (logistic regression, random forest, KNN, decision trees) on the training set.
   - Evaluated model performance using metrics such as accuracy, precision, recall, and F1-score on the testing set.
   - Compared the performance of different models to select the best one for predicting booking cancellations.

4. Model Selection :
  After evaluating multiple models, including logistic regression, random forest, K-Nearest Neighbors (KNN), and decision trees, we found that both the random forest(accuracy =95.24%)  and decision tree( accuracy = 94.97%) models provided the highest accuracy in predicting booking cancellations. However, the random forest model slightly outperformed the decision tree model in terms of accuracy. 





