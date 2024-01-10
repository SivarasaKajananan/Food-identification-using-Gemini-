# Food Calorie Estimation from Image using Gemini API

This project utilizes the Google AI Gemini Pro Vsion model to estimate the calories of individual food items presented in a given image.

Key Features
Image Analysis: Analyzes an input image to identify the food items present.
Calorie Estimation: Calculates the estimated calories for each detected food item.
Total Calorie Count: Provides a sum of the estimated calories for all food items in the image.
Technologies Used
Python
Gemini Pro vision

Installation
Install the required libraries:
pip install -q -U google-generativeai

Set up your Google API key:
from google.colab import userdata
GOOGLE_API_KEY = userdata.get('Gemini')  # Replace with your actual API key
genai.configure(api_key=GOOGLE_API_KEY)

Usage
1.Run the provided Jupyter Notebook (food_calorie_estimation.ipynb) to execute the code.
2.Upload an image of the food you want to analyze.
3.The code will process the image and generate a list of food items with their estimated calories, along with the total calorie count.
Example Output
Rice - 200 calories
Chicken - 200 calories
Dhal - 150 calories
Vegetables - 100 calories
Papadam - 100 calories
Total calories: 750 calories
   
Disclaimer
Calorie estimations are approximations and may not be entirely accurate.
The accuracy of the model depends on various factors, including image quality, food item visibility, and model limitations.
Contributing
Feel free to contribute to this project by suggesting improvements or adding new features!

# Additional Information

Model Configuration: The model is configured with specific settings for temperature, top_p, top_k, and max_output_tokens.
Safety Settings: Safety settings are configured to block content that may be harmful or offensive.
