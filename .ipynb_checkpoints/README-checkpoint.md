# Titanic Data Analysis Project 🚢

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-In%20Progress-orange)

## 📋 Table of Contents
- [Project Overview](#project-overview)
- [Objectives](#objectives)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Progress](#progress)
  - [Day 1: Initial Setup and EDA](#day-1-initial-setup-and-eda)
  - [Day 2: Advanced Analysis and Prediction](#day-2-advanced-analysis-and-prediction)
- [Setup and Installation](#setup-and-installation)
- [Key Findings](#key-findings)
- [Future Plans](#future-plans)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## 📖 Project Overview
This project is a hands-on exploration of the Titanic dataset using Python, aimed at mastering data science, machine learning, and mathematical concepts like statistics and linear algebra. It involves data preprocessing, exploratory data analysis (EDA), statistical computations, data filtering with Linux commands, and predictive modeling. The project is part of a structured learning journey to build skills in data science and machine learning.

## 🎯 Objectives
- **Data Preprocessing**: Handle missing values using statistical methods.
- **Exploratory Data Analysis**: Uncover survival patterns through visualizations.
- **Statistical Analysis**: Apply concepts like mean, standard deviation, and probability.
- **Linear Algebra**: Use matrix operations for survival predictions.
- **Linux Skills**: Practice data filtering and management with Linux commands.
- **GitHub Workflow**: Document and share progress on GitHub.

## 🗂 Dataset
The dataset is sourced from [Data Science Dojo](https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv) and contains passenger information from the Titanic:
- **Columns**: `PassengerId`, `Survived`, `Pclass`, `Name`, `Sex`, `Age`, `SibSp`, `Parch`, `Ticket`, `Fare`, `Cabin`, `Embarked`.
- **Size**: 891 rows, 12 columns.
- **Target**: `Survived` (0 = Did not survive, 1 = Survived).

## 📁 Project Structure
- `titanic.csv`: Raw dataset.
- `titanic_day1.ipynb`: Notebook for Day 1 (initial EDA and visualizations).
- `titanic_day2.ipynb`: Notebook for Day 2 (advanced analysis, missing value handling, and prediction).
- `female_passengers.csv`: Filtered dataset of female passengers.
- `male_passengers.csv`: Filtered dataset of male passengers.
- `male_under_20.txt`: Count of male passengers under 20 years old.
- `backup/`: Directory for backups of dataset and notebooks.

## 📅 Progress
### Day 1: Initial Setup and EDA
- Loaded the dataset using Pandas.
- Performed basic EDA:
  - Checked for missing values.
  - Visualized age distribution with a histogram.
- Created a backup of the dataset.
- Initialized Git repository and pushed to GitHub.

### Day 2: Advanced Analysis and Prediction
- **Missing Value Handling**:
  - Filled missing `Age` values using:
    - Overall mean.
    - Sex-based means.
    - Pclass-based means.
  - Compared distributions with histograms.
- **Statistical Analysis**:
  - Calculated overall survival probability: ~38%.
  - Computed survival probabilities by Sex (Female: ~75%, Male: ~19%).
  - Analyzed survival rates for children under 10 (~61% survival rate).
- **Data Filtering with Linux**:
  - Used `grep` and `awk` to filter female passengers and males under 20.
  - Saved results to separate files.
- **Linear Algebra**:
  - Applied matrix multiplication to predict survival scores using `Age` and `Fare`.
  - Visualized the distribution of survival scores.
- **GitHub Update**:
  - Committed changes and updated the repository.

## 🛠 Setup and Installation
### Prerequisites
- Python 3.8+
- Jupyter Notebook
- WSL2 (for Linux commands)
- Git

### Installation Steps
1. Clone the repository:
   ```bash
   git clone <your-repo-url>
   cd <your-repo-name>
   ```
2. Set up a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate
   ```
3. Install dependencies:
   ```bash
   pip install pandas numpy seaborn matplotlib
   ```
4. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
5. Open `titanic_day1.ipynb` or `titanic_day2.ipynb` to explore the analysis.

## 📊 Key Findings
- **Missing Values**: Filling `Age` based on `Pclass` resulted in a more realistic distribution compared to the overall mean, as passengers in higher classes (Pclass=1) tend to be older.
- **Survival Patterns**:
  - Women had a significantly higher survival rate (~75%) compared to men (~19%).
  - Children under 10 had a higher survival probability (~61%).
- **Prediction Insights**: Using a simple linear model with `Age` and `Fare`, higher fares were associated with better survival chances, reflecting the influence of socio-economic status.

## 🔮 Future Plans
- **Day 3**: Explore vector distances to measure passenger similarity.
- **Day 4**: Introduce derivatives for basic optimization concepts.
- **Day 5**: Analyze covariance matrices for feature correlations.
- **Long-Term**:
  - Build a logistic regression model for survival prediction.
  - Incorporate more features like `SibSp` and `Parch`.
  - Experiment with advanced ML models using PyTorch.

## 🤝 Contributing
Contributions are welcome! If you'd like to contribute:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m "Add new feature"`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a pull request.

## 📜 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments
- Dataset: [Data Science Dojo](https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv)
- Inspiration: Kaggle Titanic Challenge
- Resources:
  - [3Blue1Brown: Essence of Linear Algebra](https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab)
  - [StatQuest](https://www.youtube.com/@statquest)