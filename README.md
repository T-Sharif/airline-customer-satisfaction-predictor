# Airline Customer Satisfaction Predictor
This project uses machine learning to predict airline passenger satisfaction based on various factors related to travel experience, demographics, and service quality. By analyzing these factors, the project aims to help airlines identify key drivers of customer satisfaction and make data-driven decisions to enhance passenger experiences.

This was a group project completed for my AI and Machine Learning class—special thanks to my four teammates for their collaboration and contributions.

For a brief explanation of the program results, see the [*program_results_overview.md*](program_results_overview.md) file.

### Principal Program Objectives
Our primary objective was to use supervised learning methods to build an accurate predictive model. We aimed to:
  1. Predict customer sentiments as satisfied or dissatisfied.
  2. Identify key factors that influence passenger satisfaction.
  3. Provide actionable insights for airlines to enhance customer experiences.
  4. Enable airlines to make data-driven decisions based on the identified factors.
Additionally, our findings could contribute to the broader field of customer experience management in the airline industry, offering insights into how service quality influences customer satisfaction.

### Key Features
  1. The project leverages Python libraries including Scikit-learn, Pandas, Matplotlib, and XGBoost for data manipulation, visualization, and modeling.
  2. Insights from feature importance analysis will inform airlines of areas for service improvement, such as inflight amenities and digital boarding processes.

### Dataset
The *[Airline Passenger Satisfaction](https://www.kaggle.com/datasets/teejmahal20/airline-passenger-satisfaction)* dataset, sourced from Kaggle, contains passenger-level data with features grouped into the following categories: <br/>
&nbsp; &nbsp; **Demographics** <br/>
&nbsp; &nbsp; &nbsp; &nbsp; **Gender:** male or female <br/>
&nbsp; &nbsp; &nbsp; &nbsp; **label:** passenger's age at the time of travel <br/>

&nbsp; &nbsp; &nbsp; &nbsp; **Gender:** male or female <br/>
&nbsp; &nbsp; &nbsp; &nbsp; **Age:** passenger's age at the time of travel <br/>
&nbsp; &nbsp; &nbsp; &nbsp; **Customer Type:** loyalty status, classified as "loyal customer" or "disloyal customer" <br/>
&nbsp; &nbsp; **Flight Characteristics** <br/>
&nbsp; &nbsp; &nbsp; &nbsp; **Type of Travel:** business travel or personal travel <br/>
&nbsp; &nbsp; &nbsp; &nbsp; **Flight Distance:** distance of the flight in miles <br/>
&nbsp; &nbsp; &nbsp; &nbsp; **Class:** passenger class (Economy, Business, etc.) <br/>
&nbsp; &nbsp; **Service-Related Features** <br/>
&nbsp; &nbsp; &nbsp; &nbsp; **Inflight Wi-Fi Service:** rated on a scale from 0 to 5 <br/>
&nbsp; &nbsp; &nbsp; &nbsp; **Ease of Online Booking:** passenger's rating of the booking experience <br/>
&nbsp; &nbsp; &nbsp; &nbsp; **Convenience of Departure/Arrival Times:** ratings for the suitability of flight schedules <br/>
&nbsp; &nbsp; &nbsp; &nbsp; **Seat Comfort:** passenger rating of seating quality <br/>
&nbsp; &nbsp; &nbsp; &nbsp; **Inflight Entertainment:** passenger rating of entertainment options <br/>

The target variable, *satisfaction*, is a binary classification:
&nbsp; &nbsp; 1 = Satisfied
&nbsp; &nbsp; 0 = Neutral or Dissatisfied

### Project Steps
#### Data Preprocessing
  1. Addressed missing values, including imputing *arrival_delay_in_minutes* with the mean.
  2. Applied one-hot encoding for categorical features.
  3. Standardized numerical features like *flight_distance* and delays to ensure uniformity.

#### Exploratory Data Analysis (EDA)
  1. Analyzed the distribution of the target variable and key features.
  2. Examined correlations between features and satisfaction, highlighting strong relationships with *online_boarding*, *seat_comfort*, and *inflight_entertainment*.
  3. Visualized patterns in satisfaction across flight distance and travel type.

#### Modeling
  1. Implemented baseline models (Logistic Regression, Decision Trees) and advanced algorithms (Random Forest, XGBoost, Neural Networks).
  2. Used 5-fold cross-validation to ensure robust evaluation.
  3. Split the dataset into training (80%) and testing (20%) subsets.

#### Evaluation
  1. Assessed model performance using metrics such as accuracy, precision, recall, F1-score, and ROC-AUC.
  2. Conducted feature importance analysis to identify key predictors of satisfaction.

### Alternative Applications (Based on Code Modifications)
This project's framework can be adapted to address similar classification problems in different industries, such as:
  1. **Hotel Guest Satisfaction:** Predict customer satisfaction using factors like room quality, service, and booking convenience.
  2. **E-commerce Customer Experience:** Classify customer sentiments based on features like delivery time, product quality, and customer support.
  3. **Healthcare Patient Satisfaction:** Analyze patient feedback and experiences to identify drivers of satisfaction in medical services.
  4. **Public Transportation Feedback:** Evaluate commuter satisfaction using factors like route convenience, travel time, and service frequency.
Simple adjustments to the dataset and feature engineering process can tailor the code to these applications, enabling versatile use across domains.

Next Steps
This project serves as the foundation for exploring advanced methods to refine predictions and improve user satisfaction. Future improvements may include incorporating text analysis of customer reviews or real-time sentiment data.

