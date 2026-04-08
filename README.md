Student-Career-Recommendation-using-ANN
Student Grade Classification using Neural Networks

Project Overview This project uses a deep learning model (neural network) to predict a student's grade category based on input features such as study habits, attendance, and academic performance.

Objective The goal is to build a machine learning model that can analyze student data, learn patterns, and predict the GradeClass (0–4).

Dataset The dataset is a CSV file named student_data.csv. Example columns include:

StudentID (removed during preprocessing) StudyHours Attendance AssignmentsCompleted PreviousScore GradeClass (target variable)

Technologies Used

Python Pandas Scikit-learn TensorFlow / Keras

Workflow

Data Loading Load the dataset using pandas Data Cleaning Remove unnecessary columns such as StudentID Feature and Target Split X contains input features y contains the target variable (GradeClass) Data Scaling Normalize features using StandardScaler Train-Test Split 80 percent training data 20 percent testing data Model Building Sequential neural network with: Dense layer with 32 neurons and ReLU activation Dropout layer (0.2) Dense layer with 16 neurons and ReLU activation Dropout layer (0.2) Output layer with 5 neurons and softmax activation Model Training Epochs: 50 Batch size: 32 Prediction Predict probabilities and convert to class labels using argmax Evaluation Metrics Accuracy Precision Recall F1 Score

Model Performance The model is evaluated using accuracy, precision, recall, and F1 score to measure performance
