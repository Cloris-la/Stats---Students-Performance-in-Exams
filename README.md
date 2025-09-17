# Student Performance - Exploratory Data Analysis (EDA)

A mini data analysis project to explore and visualize the factors influencing student exam performance in mathematics, reading, and writing.

## 📖 Project Overview

This project performs an Exploratory Data Analysis (EDA) on the **"Students Performance in Exams"** dataset from Kaggle. The goal is to apply foundational data analysis and statistics skills to uncover patterns, relationships, and insights within the data.

Key steps include:
- Data loading and cleaning (handling missing values, outliers).
- Computation of descriptive statistics.
- Creation of various visualizations (histograms, box plots, scatter plots, heatmaps).
- Summarizing key findings on how factors like gender, parental education, and test preparation correlate with academic scores.

## 📊 Dataset

**Source:** [Students Performance in Exams | Kaggle]

The dataset contains the following columns:
- **`gender`**: Student's gender (male/female)
- **`race/ethnicity`**: Student's ethnic background (grouped as A, B, C, D, E)
- **`parental level of education`**: Highest education level of parents
- **`lunch`**: Type of lunch (standard/free or reduced)
- **`test preparation course`**: Whether the student completed the test prep course
- **`math score`**, **`reading score`**, **`writing score`**: Exam scores (0-100)

## 🚀 Getting Started

### Prerequisites

Before running the code, ensure you have the following installed:
- Python 3.8+
- pip (Python package manager)

### Installation & Setup

1.  **Clone the repository**
    ```bash
    git clone https://github.com/your-username/student-performance-eda.git
    cd student-performance-eda
    ```

2.  **Create a virtual environment (Recommended)**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

3.  **Install required Python packages**
    ```bash
    pip install -r requirements.txt
    ```

### Running the Analysis

The project is structured into modular scripts for a clear workflow.
Run the script to load and clean the raw data.
This will generate a `cleaned_student_performance.csv` , `descriptive_statistics_table.csv` file.All visualizations will be saved in the `/plots` directory.

**Alternatively**, you can run the entire pipeline at once using the main controller:
```bash
python main.py
📁 Project Structure
text
student-performance-eda/
│
├── data/
│   ├── studentsperformance.csv       # Original dataset (add manually)
│   └── cleaned_student_performance.csv  # Generated cleaned data
│
├── plots/                            # Generated visualizations
│   ├── hist_math_score.png
│   ├── box_math_score_by_gender.png
│   └── comprehensive_association_heatmap.png
├── src.ipynb
├── requirements.txt
├── .gitignore
└── README.md
🔍 Key Insights Summary
Test Preparation: Completing the test preparation course is strongly associated with higher scores across all three subjects.

Gender Gap: Female students tend to outperform male students in Reading and Writing, while male students show greater variability in Math scores.

Socioeconomic Factors: Parental education level and lunch type (a potential proxy for socioeconomic status) show a positive correlation with student performance.

High Correlation: Scores in Math, Reading, and Writing are highly correlated. A student strong in one subject is likely strong in the others.

For a detailed report with all charts and findings, please refer to the generated plots and the comments within the Jupyter Notebook (analysis_notebook.ipynb), if provided.