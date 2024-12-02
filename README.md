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
This project was completed as part of the LearnBay "Advanced Data Science and AI" course. The dataset used for this hands-on assessment was provided by the course instructors, so the exact source of the dataset is unknown.

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

---

## Packages Used 📦
## Libraries and Packages Used

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

## Steps :stairs:

