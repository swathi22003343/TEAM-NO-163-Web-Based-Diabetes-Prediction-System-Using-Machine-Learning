# TEAM.NO.163 : Web-Based Diabetes Prediction System Using Machine Learning

## About

This project aims to provide an accessible tool for predicting the risk of diabetes, leveraging machine learning algorithms integrated into a web-based interface. Users can input health data, and the system returns real-time predictions about their diabetes risk. This proactive approach can help individuals make informed decisions about their health and seek medical advice if necessary.

## Features

- Data Input Interface: Users can enter health metrics such as age, BMI, blood pressure, and cholesterol.
- Real-Time Predictions: The system uses a trained machine learning model to predict diabetes risk.
- Multiple Models: Compares several models to select the most effective one, ensuring optimal prediction accuracy.
- User-Friendly Interface: Designed for ease of use by both technical and non-technical users.

## Development Requirements

- Operating System: 64-bit OS (Windows 10, macOS, Ubuntu).
- Development Environment: Python 3.10+.
- Machine Learning Libraries: Scikit-learn for model implementation and evaluation.
- Frameworks and Tools: Django for backend development, Flask for API integration, and HTML/CSS for frontend.
- Additional Dependencies: NumPy, Pandas for data handling, and Matplotlib for visualizing results.

## System Architecture

![Screenshot 2024-10-29 190230](https://github.com/user-attachments/assets/0ed55d70-04e9-45d3-ac5e-86b4581426a6)

- Frontend: HTML5, CSS3, and JavaScript.
- Backend: Django-based backend for request handling and model integration.
- Model: A Decision Tree model optimized for accuracy and interpretability.

## Methodology

1.Data Preprocessing:

   i)Cleaning data by removing duplicates and handling missing values.

   ii)Selecting key features, including age, BMI, blood pressure, and cholesterol, as predictors.
    
2.Model Training:

   i)Multiple algorithms were trained, including Decision Tree, Random Forest, and Gradient Boosting, to determine the most effective model.
    
   ii)The Decision Tree model achieved the highest accuracy, making it ideal for deployment in this application.
    
3.Model Evaluation:

   - Evaluated using accuracy, precision, recall, and F1-score.
   - The Decision Tree model demonstrated balanced performance and interpretability.
     
![Screenshot 2024-10-30 013354](https://github.com/user-attachments/assets/c9a79388-5947-4e7e-b313-c2c7e24bfe22)

![Screenshot 2024-10-30 013413](https://github.com/user-attachments/assets/2f8d3456-9dfe-48a1-9641-2024b9df79e8)

## Setup Instructions

- Run the Django Server:
```
python manage.py runserver
```
- Access the Web Interface: Visit http://127.0.0.1:5000/ in your web browser.

## Project Structure
- app.py: Main Python file where the Flask application is initialized. It will include routes to handle form submissions, load the model, and display results.
- data/diabetics.csv: Folder to store the dataset used for training the model.
- model/diabetics.pkl: Folder to store the trained model as a .pkl file for easy loading and usage within the app.
- static/: Contains static files such as images (diabetics1.jpeg and diabetics2.jpeg), as well as CSS and JavaScript files, if needed.
- templates/: Contains HTML templates. index.html is the main input page, and result.html shows the prediction output.
               
## Results

The Decision Tree model achieved an accuracy of approximately 92%, making it effective for predicting diabetes risk in a non-clinical setting. This accuracy enables users to gain valuable insights into their health status, encouraging early action and potentially preventing severe complications associated with diabetes.

## Output 
### Web-page asking for input from user
![WhatsApp Image 2024-10-30 at 12 21 46 AM](https://github.com/user-attachments/assets/c9ec856f-7faf-4a92-839d-51393736528e)

### Web-page displays the result
![WhatsApp Image 2024-10-30 at 12 21 46 AM (1)](https://github.com/user-attachments/assets/19a02e2c-3482-48da-beab-e21c16934673)

## Future Improvements

  - Expand Feature Set: Incorporate additional health indicators, such as family history and genetic data.
  - Model Refinement: Experiment with ensemble methods to further improve prediction accuracy.
  - Enhanced User Interface: Introduce data visualization for better user engagement.
    
## References

 - Victor, K. F., & Michael, I. Z. (2018). Intelligent data analysis and machine learning: Are they really equivalent concepts? Springer-Verlag.
 - John, L. A., & Rose, M. B. (2021). Early Detection of Diabetes Using Machine Learning Algorithms. CRC Press.
 - Clarke, R. S., & Emerson, N. T. (2020). Diabetes Prediction Using Machine Learning Techniques: A Comparative Study of Algorithms. Wiley.
 - Mitchell, D. R., & Thomson, A. E. (2022). Diabetes Mellitus Prediction Using Machine Learning Techniques: A Comprehensive Review. Elsevier.
