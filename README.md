# Titanic Dataset Preprocessing (Task 1)

## Objective
Clean and prepare the Titanic dataset for machine learning using Jupyter Notebook.

## Steps
1. Loaded and explored the dataset (checked missing values, data types).
2. Fixed missing values:
   - Filled `Age` with median (28).
   - Filled `Embarked` with mode (‘S’).
   - Dropped `Cabin`, `PassengerId`, `Name`, `Ticket`.
3. Converted text to numbers:
   - `Sex`: male=0, female=1.
   - `Embarked`: Created `Embarked_C`, `Embarked_Q` columns.
4. Standardized `Age`, `Fare`, `SibSp`, `Parch` to have mean=0, std=1.
5. Visualized outliers with boxplots for `Age` and `Fare` before and after removing outliers for both columns using the IQR method (final shape: 718 rows).

## Files
- `ElevateLabs Task1.ipynb`: Jupyter Notebook with code.
- `Titanic-Dataset.csv`: Original dataset.
- `cleaned_titanic.csv`: Cleaned dataset (718 rows, 9 columns).
- `boxplots_before.png`: Boxplots for `Age` and `Fare` before outlier removal.
- `boxplots_after.png`: Boxplots for `Age` and `Fare` after outlier removal.

## Tools
- Jupyter Notebook, Python, Pandas, NumPy, Matplotlib, Seaborn, scikit-learn

## How to Run
1. Install libraries: `pip install pandas numpy matplotlib seaborn scikit-learn`
2. Place `Titanic-Dataset.csv` in the same folder as the notebook.
3. Open and run `titanic_preprocessing.ipynb` in Jupyter Notebook.
