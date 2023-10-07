# Heart-Disease-Prediction
# Heart Disease Prediction Dataset

## Overview

This dataset contains various attributes related to patients' health, including demographic information and medical parameters. The goal is to predict the presence or absence of heart disease in patients. The dataset originally had 76 attributes, but experiments and machine learning research have focused on a subset of 14 attributes. The "target" field represents the presence of heart disease and is integer-valued from 0 (no presence) to 4. For most experiments, presence (values 1, 2, 3, 4) and absence (value 0) of heart disease have been the primary focus.

## Dataset Details

### Features

1. **age**: Age of the patient (in years)
2. **sex**: Gender of the patient (1 = male, 0 = female)
3. **cp**: Chest pain type
    - 1: Typical angina
    - 2: Atypical angina
    - 3: Non-anginal pain
    - 4: Asymptomatic
4. **trestbps**: Resting blood pressure (in mm Hg)
5. **chol**: Serum cholesterol level (in mg/dl)
6. **fbs**: Fasting blood sugar > 120 mg/dl (1 = true; 0 = false)
7. **restecg**: Resting electrocardiographic results
    - 0: Normal
    - 1: Having ST-T wave abnormality
    - 2: Showing probable or definite left ventricular hypertrophy
8. **thalach**: Maximum heart rate achieved
9. **exang**: Exercise-induced angina (1 = yes; 0 = no)
10. **oldpeak**: ST depression induced by exercise relative to rest
11. **slope**: Slope of the peak exercise ST segment
    - 1: Upsloping
    - 2: Flat
    - 3: Downsloping
12. **ca**: Number of major vessels colored by fluoroscopy (0-3)
13. **thal**: Thalassemia
    - 3: Normal
    - 6: Fixed defect
    - 7: Reversible defect

### Target

- **num**: Diagnosis of heart disease
    - 0: < 50% diameter narrowing (no heart disease)
    - 1: > 50% diameter narrowing (presence of heart disease)

## Attribute Information

- **id**: Patient identification number
- **ccf**: Social security number (replaced with dummy value 0)
- **painloc**: Chest pain location (1 = substernal; 0 = otherwise)
- **painexer**: Chest pain provoked by exertion (1 = yes; 0 = no)
- **relrest**: Chest pain relieved after rest (1 = yes; 0 = no)
- **pncaden**: Sum of painloc, painexer, and relrest
- **htn**: History of hypertension (1 = yes; 0 = no)
- **smoke**: Smoking status (1 = yes; 0 = no)
- **cigs**: Number of cigarettes smoked per day
- **years**: Number of years as a smoker
- **dm**: History of diabetes (1 = yes; 0 = no)
- **famhist**: Family history of coronary artery disease (1 = yes; 0 = no)
- **ekgmo**: Month of exercise ECG reading
- **ekgday**: Day of exercise ECG reading
- **ekgyr**: Year of exercise ECG reading
- **dig**: Digitalis used during exercise ECG (1 = yes; 0 = no)
- **prop**: Beta blocker used during exercise ECG (1 = yes; 0 = no)
- **nitr**: Nitrates used during exercise ECG (1 = yes; 0 = no)
- **pro**: Calcium channel blocker used during exercise ECG (1 = yes; 0 = no)
- **diuretic**: Diuretic used during exercise ECG (1 = yes; 0 = no)
- **proto**: Exercise protocol
    - 1: Bruce
    - 2: Kottus
    - 3: McHenry
    - 4: Fast Balke
    - 5: Balke
    - 6: Noughton
    - 7: Bike 150 kpa min/min
    - 8: Bike 125 kpa min/min
    - 9: Bike 100 kpa min/min
    - 10: Bike 75 kpa min/min
    - 11: Bike 50 kpa min/min
    - 12: Arm ergometer
- **thaldur**: Duration of exercise test in minutes
- **thaltime**: Time when ST measure depression was noted
- **met**: METs achieved
- **thalsev**: Not used
- **thalpul**: Not used
- **earlobe**: Not used
- **cmo**: Month of cardiac catheterization (sp?)
- **cday**: Day of cardiac catheterization (sp?)
- **cyr**: Year of cardiac catheterization (sp?)
- **lmt**, **ladprox**, **laddist**, **diag**, **cxmain**, **ramus**, **om1**, **om2**, **rcaprox**, **rcadist**: Not used
- **lvx1**, **lvx2**, **lvx3**, **lvx4**, **lvf**, **cathef**, **junk**: Not used

## Repository Contents

- **data**: Folder containing the dataset files.
    - **heart_disease_data.csv**: Main dataset file.
    - **attribute_details.txt**: Detailed description of dataset attributes.
- **notebooks**: Jupyter notebooks for data exploration, preprocessing, and modeling.
    - **Exploratory_Data_Analysis.ipynb**: Notebook for exploring the dataset.
    - **Data_Preprocessing.ipynb**: Notebook for preprocessing the data.
    - **Model_Training_and_Evaluation.ipynb**: Notebook for training machine learning models and evaluating performance.
- **src**: Source code files.
    - **data_loader.py**: Python script for loading the dataset.
    - **preprocessing.py**: Python script for preprocessing the data.
    - **model.py**: Python script containing machine learning models.
- **requirements.txt**: File specifying the required Python packages and their versions.
- **README.md**: Readme file providing an overview of the repository and instructions for usage.

## How to Use

1. **Clone the Repository**: Clone this repository to your local machine using `git clone https://github.com/your-username/heart-disease-prediction.git`.
2. **Navigate to Repository**: `cd heart-disease-prediction`.


3. **Create Virtual Environment (Optional)**: Create a virtual environment using `virtualenv venv` and activate it (commands may vary based on your OS).
4. **Install Dependencies**: Install the required packages using `pip install -r requirements.txt`.
5. **Explore Notebooks**: Use Jupyter notebooks in the `notebooks` folder for data exploration, preprocessing, model training, and evaluation.
6. **Run Python Scripts**: Utilize Python scripts in the `src` folder for specific tasks (e.g., data loading, preprocessing, modeling).
7. **Experiment and Contribute**: Feel free to experiment with different models and techniques. Contributions and improvements are welcome!

## Dataset Source

The original dataset is sourced from [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Heart+Disease). Please refer to the UCI repository for detailed information about the dataset and its source.

If you have any questions or need assistance, please feel free to reach out. Happy coding!
