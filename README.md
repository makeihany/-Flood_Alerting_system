This is a lightweight flood prediction software using #machinelearning in #pythonprogramminglanguage. 

The software comprises three distinct files:

1- Model.py: This file utilizes a Random Forest Regressor to calculate flood probabilities, trained on historical data including rainfall, river discharge, and previous floods. It achieved optimal Mean Squared Error and R2 Score. The model accepts current rainfall and discharge data as input and outputs a table of high-risk stations. Libraries used include #pandas, #numpy, #sklearn, and #pyodbc.

2- app.py: This file processes the table array generated by Model.py and, with the #flask framework and #folium library, creates a Google Maps-compatible list of station markers for display.

3- index.html: Serving as the UI, this file represents the app.py output, displaying flood-prone stations with color-coded markers ranging from green to red, representing flood probability percentages. A text box alongside each marker provides the percentage value.
