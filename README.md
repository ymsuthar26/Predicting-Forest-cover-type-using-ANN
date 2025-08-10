# Predicting-Forest-cover-type-using-ANN
This project predicts the type of forest cover using the Covertype dataset from scikit-learn, implementing an Artificial Neural Network (ANN) with TensorFlow/Keras. The workflow covers data preprocessing, scaling, model design, and performance evaluation.
# Dataset
The Covertype dataset contains cartographic variables (elevation, slope, soil type, etc.) to classify forest cover type into 7 different categories.

Features: 54
Target: Forest cover type (integer labels 1–7)

# Library Used
Pandas, NumPy
Matplotlib, Seaborn
Scikit-learn
TensorFlow / Keras

Project Workflow
1. Data Loading
Fetched the Covertype dataset using fetch_covtype() from scikit-learn.
Stored features in X and target in y
2. Data Exploration
Checked for null values and duplicates.
Reviewed unique class distribution in the target variable.
3. Data Preprocessing
Standardized features using StandardScaler to normalize inputs.
Stratified train-test split (75% training, 25% testing).
4. Model Building (ANN)
Input Layer: 256 neurons, ReLU activation, Dropout 0.4.
Hidden Layer 1: 128 neurons, ReLU activation, Dropout 0.3.
Hidden Layer 2: 64 neurons, ReLU activation, Dropout 0.3.
Output Layer: 8 neurons (softmax activation for multi-class classification).
5. Compilation & Training
Optimizer: Adam
Loss: Sparse Categorical Crossentropy
Metrics: Accuracy
6. Evaluation
Model summary displayed.
Accuracy measured on the test dataset.
# Results
Final Test Accuracy: (Add final accuracy here after training)

Model successfully classifies the forest cover type with good accuracy using ANN.
