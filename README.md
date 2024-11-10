# RANDOMFOREST
Random forest from scratch using IG and Entropy on titanic dataset and Gini Index for sona dataset
---

# Random Forest from Scratch

Custom Random Forest classifier using:
- **Information Gain (IG) and Entropy** on the Titanic dataset
- **Gini Index** on the Sona dataset

## Structure

- `data/titanic.csv` & `data/sona.csv`: Datasets
- `src/random_forest.py`: Random Forest implementation
- `README.md`: Instructions
- `requirements.txt`: Dependencies

## Installation

```bash
git clone https://github.com/Setsofia-lab/RANDOMFOREST.git
cd random-forest-scratch
pip install -r requirements.txt
```

## Usage

1. **Train Classifier**:
   ```python
   from src.random_forest import RandomForestClassifier
   rf = RandomForestClassifier(criterion='entropy')  # Use 'gini' for Sona dataset
   rf.fit(X_train, y_train)
   ```

2. **Predict & Evaluate**:
   ```python
   predictions = rf.predict(X_test)
   accuracy = rf.evaluate(y_test, predictions)
   print(f"Accuracy: {accuracy * 100:.2f}%")
   ```
