# Cleveland Cavaliers With and Without LeBron James

An analysis of Cleveland Cavaliers season stats (39 seasons) comparing the team with and without LeBron James. It includes correlation analysis and classification models that predict whether LeBron was on the roster.

## Repository Contents

| File | Description |
|---|---|
| `Lebron Cavs Machine Learning .ipynb` | Full analysis: correlations and classification models |
| `ClevelandCavs.csv` | Season-level team stats: wins, losses, points, shooting, rebounds, assists, steals, turnovers and fouls |

## Commit History

### `1a7a494`: Upload of the notebook and dataset (2022-05-18)
- **Correlation analysis:**
  - little or no relationship between wins and points, points per game, field goal percentage, rebounds, assists or free-throw shooting
  - with LeBron on the roster, the Cavs turned the ball over less and committed fewer fouls
- **Classification: predicting whether LeBron was on the Cavs** from wins, losses, points, field goals, free throws, rebounds, assists, steals, turnovers and fouls, with feature scaling, a train/test split (10 test seasons) and confusion-matrix analysis:

  | Model | Accuracy |
  |---|---|
  | Logistic regression | 80% |
  | Naive Bayes | 90% |
  | K-nearest neighbors | 90% |
  | Kernel SVM | 90% |
  | Decision tree | 80% |
  | Random forest | 90% |
  | **SVM (10-fold cross-validation and grid search, best)** | **96.67%** |

## Tools
Python, pandas, NumPy, scikit-learn, matplotlib, seaborn, Jupyter Notebook
