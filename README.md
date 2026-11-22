# Student Performance Analysis

An end-to-end data analysis, visualization, and machine learning project built in Python to explore how attendance, study habits, and continuous assessments impact student academic performance.

## Project Workflow

1. **Synthetic Dataset Generation**: Simulates realistic records for 500 students including attendance, study hours, sleep hours, revision habits, group study, and exam scores (`Assignment`, `Quiz`, `Midterm`, `FinalScore`).
2. **Data Cleaning & Feature Engineering**: Handles missing values via median imputation, removes duplicates, categorizes attendance levels, and assigns final grades (`A`, `B`, `C`, `Fail`).
3. **Exploratory Data Analysis (EDA)**: Computes summary statistics, pass percentages, group-wise performance averages, and feature correlations.
4. **Data Visualization**: Generates 11 analytical charts saved inside the `graphs/` directory.
5. **Machine Learning (From Scratch in NumPy)**:
   - **Linear Regression** (Ordinary Least Squares) to predict `FinalScore`, evaluated with R² and Mean Absolute Error (MAE).
   - **Logistic Regression** (Gradient Descent) to classify `Pass`/`Fail` outcomes, evaluated with accuracy, a confusion matrix, and feature importance weights.

## Repository Structure

```text
student_performance_analysis/
├── student_performance_analysis.py   # Main analysis, visualization & ML script
├── student_data_cleaned.csv          # Cleaned dataset exported by the script
├── graphs/                           # 11 generated PNG visualizations
│   ├── 1_score_distribution.png
│   ├── 2_attendance_vs_score.png
│   ├── 3_studyhours_vs_score.png
│   ├── 4_revision_effect.png
│   ├── 5_attendance_level_boxplot.png
│   ├── 6_assessment_averages.png
│   ├── 7_grade_pie.png
│   ├── 8_correlation_heatmap.png
│   ├── 9_actual_vs_predicted.png
│   ├── 10_confusion_matrix.png
│   └── 11_feature_importance.png
└── README.md
```

## Sample Visualizations

| Score Distribution | Correlation Heatmap |
| :---: | :---: |
| ![Score Distribution](graphs/1_score_distribution.png) | ![Correlation Heatmap](graphs/8_correlation_heatmap.png) |

| Actual vs Predicted | Feature Importance |
| :---: | :---: |
| ![Actual vs Predicted](graphs/9_actual_vs_predicted.png) | ![Feature Importance](graphs/11_feature_importance.png) |

## How to Run Locally

1. **Clone the repository:**
   ```bash
   git clone https://github.com
   cd student_performance_analysis
   ```

2. **Install dependencies:**
   ```bash
   pip install numpy pandas matplotlib seaborn
   ```

3. **Run the script:**
   ```bash
   python student_performance_analysis.py
   ```

## Tech Stack
* **Python 3**
* **NumPy** & **Pandas** (Data manipulation & custom ML algorithms)
* **Matplotlib** & **Seaborn** (Statistical visualizations)
