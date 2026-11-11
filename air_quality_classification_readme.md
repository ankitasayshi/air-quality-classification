# 1. Air Quality Classification

## 2. Project Overview

This project focuses on classifying air quality using machine learning techniques.

## 3. Problem Statement:
Air Quality Classification Using Environmental and Pollution Indicators using logistic regression


## 4. Dataset Description
The project uses the Air Quality and Pollution Assessment dataset published by Mujtaba Matin on Kaggle.  
**Dataset Source:** Kaggle – Air Quality and Pollution Assessment  
The dataset contains environmental and pollution-related parameters that can be used to analyse and classify air quality.  
**Source:** https://www.kaggle.com/datasets/mujtabamatin/air-quality-and-pollution-assessment

### Features Description

| Feature | Description |
| :--- | :--- |
| **Temperature** | Atmospheric temperature |
| **Humidity** | Relative humidity |
| **PM2.5** | Concentration of fine particulate matter |
| **PM10** | Concentration of particulate matter |
| **NO2** | Nitrogen dioxide concentration |
| **SO2** | Sulphur dioxide concentration |
| **CO** | Carbon monoxide concentration |
| **Proximity_to_Industrial_Areas** | Proximity to industrial areas |
| **Population_Density** | Population density |
| **Air Quality** | Target classification variable |

### Target Variable:
The target variable is **Air Quality**, which represents the air quality category.  
The listed classification categories are:
- Good
- Moderate
- Poor
- Hazardous

### Dataset Characteristics
- **Format:** CSV
- **Expected observations:** Approximately 5,000
- **Expected columns:** 10
- **Problem type:** Multiclass Classification
- **Target variable:** Air Quality

The dataset will be explored to understand feature distributions, identify missing values, analyse relationships between variables and prepare the data for machine learning.

## 5. Methodology

The dataset is loaded from the CSV file using the Pandas library.

Initial inspection is performed to understand:
- Number of rows and columns.
- Feature names and data types.
- Missing values and duplicate records.
- Distribution of target classes.

### 5.2 Exploratory Data Analysis (EDA)

Exploratory Data Analysis is performed to understand the characteristics and patterns present in the dataset.

The analysis includes:
- Statistical summary of numerical features.
- Distribution of pollution-related parameters.
- Correlation analysis between numerical features.
- Visualisation of air quality class distribution.
- Identification of possible outliers.

Libraries such as Matplotlib and Seaborn are used for data visualisation.

### 5.3 Data Preprocessing

The dataset is prepared before applying Machine Learning algorithms.

The preprocessing stage may include:
- **Missing Value Handling:** Identifying and handling missing observations.
- **Duplicate Removal:** Checking for repeated records.
- **Categorical Encoding:** Converting categorical variables into numerical representations wherever required.
- **Feature Scaling:** Applying normalization or standardization when appropriate.
- **Feature Selection:** Identifying relevant features that contribute to air quality classification.

All preprocessing decisions will be based on the actual dataset.

### 5.4 Feature Selection and Target Separation

The input features are separated from the target variable.
- **Input (X):** Environmental and pollution-related parameters.
- **Output (y):** Air Quality.

The target variable represents the category that the model is expected to predict.

### 5.5 Train-Test Split

The dataset is divided into two subsets:
- **Training Set:** Used to train the Machine Learning model.
- **Testing Set:** Used to evaluate the model on unseen data.

The train-test split helps assess the model's ability to generalize to new observations.

### 5.6 Model Training

The selected Machine Learning classification algorithm is trained using the prepared training dataset.

The model learns patterns and relationships between environmental parameters and their corresponding air quality categories.

*Selected Algorithm:* To be updated after the final model is confirmed.

### 5.7 Model Evaluation

The trained model is evaluated using appropriate classification metrics:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

These metrics help assess the model's classification performance and identify the types of prediction errors it makes.


## 6. Team Members

- **2026EEB1322** ANKITA SAINI - DOCUMMENTATION LEAD
- **2026AIB1095** VENNA DIVIJA - PPT LEAD
- **2026EEB1393** PRANJAL - EXECUTIVE LEAD
- **2026MCB1569** SHIVANSH VAISH - VIDEO LEAD


## 7. Project Structure
The GitHub repository is organized to keep the project files accessible and easy to understand.

```text
air-quality-classification/
│
├── README.md
│
├── dataset.csv
│
├── main.ipynb
│
├── requirements.txt
│
├── presentation.pdf
│
└── video_link.txt
```

### Description of Files

| File | Purpose |
| :--- | :--- |
| `README.md` | Project overview, methodology and execution instructions |
| `updated_pollution_dataset[1].csv` | Dataset used for model development |
| `main.ipynb` | Jupyter Notebook containing the complete ML workflow |
| `requirements.txt` | List of required Python libraries |
| `presentation.pdf` | Five-slide project presentation |
| `video_link.txt` | Link to the project demonstration video |

-The repository is maintained on GitHub and made publicly accessible for evaluation  
**BY DOCUMMENTATION LEAD, 2026EEB1322**


## Installation and Requirements

### Prerequisites:
The following software and tools are required to execute the project:
- Python 3.x
- Jupyter Notebook
- pip (Python package installer)
- Git (for cloning the repository)

### Required Python Libraries
The project uses Python libraries for data manipulation, visualization and Machine Learning.

| Library | Purpose |
| :--- | :--- |
| **NumPy** | Numerical computations |
| **Pandas** | Data loading and manipulation |
| **Matplotlib** | Data visualization |
| **Seaborn** | Statistical visualization |
| **Scikit-learn** | Data preprocessing, model training and evaluation |

### Installation Steps

**Step 1:** Clone the GitHub repository
```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

**Step 2:** Navigate to the project directory
```bash
cd air-quality-classification
```

**Step 3:** Install the required dependencies
```bash
pip install -r requirements.txt
```

**Step 4:** Launch Jupyter Notebook
```bash
jupyter notebook
```
The project notebook can then be opened in the browser.



## How to Run
Follow these steps to execute the Air Quality Classification project:

1. Download or clone the public GitHub repository.
2. Ensure that Python and the required dependencies are installed.
3. Install all dependencies using the `requirements.txt` file.
4. Ensure that the dataset CSV file is present in the correct project directory.
5. Launch Jupyter Notebook.
6. Open `main.ipynb`.
7. Execute the notebook cells sequentially, starting from the first cell.
8. Observe the data preprocessing steps, model training process and evaluation results.

### Execution Command
```bash
jupyter notebook main.ipynb
```
Alternatively, the notebook can be opened through Jupyter's browser interface.

### Expected Output
After successful execution, the notebook should display:
- Dataset overview and exploratory analysis.
- Data preprocessing results.
- Training and testing dataset information.
- Trained classification model.
- Model evaluation metrics.
- Confusion matrix and relevant visualizations.

The final output will demonstrate the model's ability to classify air quality into the categories represented in the dataset.


## Results and Evaluation
The trained model will be evaluated using suitable classification metrics.

The final results will include:
- Accuracy score.
- Precision score.
- Recall score.
- F1-score.
- Confusion matrix.
- Relevant training and evaluation plots.

The results will be interpreted to understand the model's performance and its effectiveness in classifying air quality.

### Model Performance:

Two machine learning classification models were implemented and evaluated:
1. Logistic Regression
2. Random Forest Classifier

The models were evaluated on a testing dataset containing 1,000 samples.

| Evaluation Metric | Logistic Regression | Random Forest |
| :--- | :--- | :--- |
| **Accuracy** | 93% | 95.1% |
| **Weighted Precision** | 0.93 | 0.95 |
| **Weighted Recall** | 0.93 | 0.95 |
| **Weighted F1-Score** | 0.93 | 0.95 |

### Classification Performance

The models classify air quality into four categories:
- Good
- Moderate
- Poor
- Hazardous

### Random Forest Classification Report:

| Air Quality Class | Precision | Recall | F1-Score |
| :--- | :--- | :--- | :--- |
| **Good** | 1.00 | 1.00 | 1.00 |
| **Hazardous** | 0.90 | 0.80 | 0.85 |
| **Moderate** | 0.96 | 0.97 | 0.97 |
| **Poor** | 0.87 | 0.90 | 0.88 |

### Evaluation and Observations
- Random Forest achieved the highest accuracy of approximately 95.1%, outperforming Logistic Regression.
- Random Forest performed particularly well in classifying Good and Moderate air quality.
- Hazardous air quality had a comparatively lower recall of 0.80, indicating that some hazardous samples were incorrectly classified.
- Logistic Regression achieved approximately 93% accuracy, demonstrating good classification performance.
- Overall, Random Forest was selected as the best-performing model among the two evaluated models.

### Conclusion
The experimental results demonstrate that machine learning techniques can effectively classify air quality into different categories. Random Forest provided better overall performance than Logistic Regression on the testing dataset and was selected as the final model.


## Presentation and Video:
To be added.

## AI Usage Disclosure:
AI tools were used as supportive resources during the development and documentation of this project.

The use of AI was limited to the following activities:
- **Concept Clarification:** Understanding machine learning concepts, classification techniques, and model evaluation metrics.
- **Documentation Assistance:** Improving the structure, readability, and presentation of the README file.
- **Code Understanding:** Assisting in understanding Python libraries, code functionality, and machine learning workflows.
- **Debugging Support:** Helping identify and resolve coding errors during development.

The dataset selection, project implementation, model training, testing, evaluation, and final verification were carried out by the project team.

AI-generated suggestions were reviewed and adapted by the team to ensure their correctness and relevance.

AI tools were used to support learning and development, not to replace the team's understanding or contribution.