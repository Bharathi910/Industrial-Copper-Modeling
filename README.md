# Industrial-Copper-Modeling

**video**

https://www.linkedin.com/posts/siva-bharathi-n-9b233b1b4_guvi-machinelearning-datascience-activity-7224772945154338816-UfOn?utm_source=share&utm_medium=member_desktop

**Libraries**

**Streamlit:** For creating the web interface.

**Option Menu:** For navigation in the web app.

**Datetime, Pandas, Numpy:** For data manipulation and date handling.

**Seaborn, Matplotlib:** For data visualization (although not used in the code).

**Warnings:** To ignore warnings.

**Pickle:** For loading pre-trained models and encoders.

**Scikit-learn:** For machine learning tasks.

**Streamlit Configuration**

The page is configured with a title, icon, and layout settings.
Custom CSS is added to set the background image of the page.
A header is displayed at the top of the page.
Navigation
An option menu is created with three tabs: "HOME", "PRICE PREDICTION", and "STATUS PREDICTION".

**Home Page**

Displays the problem statement and an overview of the models used:
Regression Model: ExtraTreeRegressor
Classification Model: RandomForestClassifier

**Price Prediction**

Takes input from the user for various features such as quantity, thickness, width, country, status, item type, application type, product reference, order date, and delivery date.
Uses pre-trained models and encoders to predict the selling price of copper.
Displays the predicted price to the user.

**Status Prediction**

Takes input from the user for features similar to those used in price prediction but includes the selling price.
Uses pre-trained models and encoders to predict the status of the deal.
Displays whether the status is "WON" or "LOST".

**Error Handling**

In both prediction sections, there are try-except blocks to handle errors if the user does not fill in all required fields.

**Key Functions**

**Label Encoding:** Used to encode categorical variables such as country, status, and item type.

**Model Prediction:** Uses pre-trained models (loaded with pickle) to make predictions based on user inputs.

**Date Handling:** Calculates the difference between the order date and delivery date.

**Example Outputs**

**Predicted Price:** Displayed as a success message with the predicted value.

**Predicted Status:** Displayed as a success message for "WON" or an error message for "LOST".
