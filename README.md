# AggriAssist
AgriAssist is a data-driven, command-line application (CLI) built in Python. Its goal is to provide actionable insights for farmers and transparent pricing information for customers. The project leverages a machine learning model for predictive analysis and a rule-based system for generating specific, real-time advice on crop management.
✅ Core Features Implemented
The project has successfully reached a functional proof-of-concept stage with the following key features fully implemented:

Dual-User System: The application has two distinct modes: a Farmer Mode for crop management and a Customer Mode for market analysis.

Machine Learning Integration: A Random Forest Classifier is trained and used to predict the Crop_Health_Status ("Good" or "Bad") based on environmental and farm-input data.

Comprehensive Farmer Recommendations:

Irrigation Advice: Provides clear actions based on soil moisture levels.

Pest Management: Offers basic guidance on pest control.

Detailed Fertilizer Detection: A key feature has been added to provide specific fertilizer recommendations (e.g., "Urea," "Potash," "NPK") based on the crop type, its current growth stage, and the detected soil fertility.

Economic Analysis:

For farmers, it calculates a fair sale price and estimates the profit per acre.

For customers, it calculates potential savings compared to standard market prices.

Interactive CLI: The entire application runs in the terminal, guiding the user with prompts for necessary inputs.

## 📈 Analysis of Current State
The application's logic is sound and the end-to-end workflow—from data input to generating a full report—is complete and functional.

However, the project's main limitation is its reliance on simulated and static data. The ML model is trained on a very small (10-entry) sample dataset, which means its predictions are not yet reliable for real-world use. Similarly, the "scan" feature uses random numbers, and all market data is hardcoded.

## 🚀 Recommended Next Steps
The foundational logic is solid, making the project ready for the next phase of development. The following steps would move AgriAssist from a proof-of-concept to a viable tool:

Improve the ML Model: Train the RandomForestClassifier on a large, real-world agricultural dataset to dramatically improve prediction accuracy.

Transition to a Web Application: Rebuild the user interface using a framework like Flask or Streamlit. This will make the tool more accessible and user-friendly than the current command-line version.

Integrate Real-Time Data: Connect the application to external APIs to fetch live weather data and dynamic market prices for crops.

Implement a Database: Add a database (like SQLite or PostgreSQL) to store historical data from scans, track crop performance over time, and potentially personalize recommendations for specific farms.
