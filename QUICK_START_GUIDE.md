# 🚀 DAY 1 QUICK START GUIDE

## ⏱️ Time Estimate: 30 minutes setup + 2-3 hours execution

---

## Step 1: Download Files ✅

You've received 3 files:
1. `Bank_Churn_Prediction.ipynb` - **Main notebook** with all code
2. `README.md` - Project documentation
3. `requirements.txt` - Python dependencies

---

## Step 2: Setup Your Environment

### On Windows:
```bash
# Create a new folder for the project
mkdir bank-churn-prediction
cd bank-churn-prediction

# Create virtual environment (optional but recommended)
python -m venv venv
venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter
jupyter notebook
```

### On Mac/Linux:
```bash
# Create a new folder for the project
mkdir bank-churn-prediction
cd bank-churn-prediction

# Create virtual environment (optional but recommended)
python3 -m venv venv
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter
jupyter notebook
```

---

## Step 3: Open the Notebook

1. Jupyter will open in your browser (usually http://localhost:8888)
2. Navigate to and click on `Day_01_Bank_Churn_Prediction.ipynb`
3. The notebook will open in the browser

---

## Step 4: Run the Notebook (Section by Section)

The notebook is organized into 10 sections:

### **SECTION 0: Setup & Imports** ⏱️ 2 minutes
- Run all cells to import libraries
- You'll see: `✅ All libraries imported successfully!`

### **SECTION 1: Download & Load Dataset** ⏱️ 5 minutes
- **First time running?** The notebook will download the dataset automatically
- Look for: `✅ Dataset downloaded successfully!`
- **Already downloaded?** Just load the CSV

**✋ IMPORTANT - Two Options:**
- **Option A (Automatic)**: Let the notebook download the dataset (easiest)
- **Option B (Manual)**: 
  1. Go to https://www.kaggle.com/datasets
  2. Search: "Bank Customer Churn"
  3. Download CSV
  4. Place in project folder
  5. Run the notebook

### **SECTION 2: Data Exploration** ⏱️ 10 minutes
- See dataset structure, columns, data types
- Look for patterns in the data
- **Output**: Overview statistics and information

### **SECTION 3: Data Cleaning** ⏱️ 10 minutes
- Remove unnecessary columns
- Encode categorical variables (convert text to numbers)
- Handle outliers
- **Output**: Cleaned dataset ready for analysis

### **SECTION 4: EDA (Exploratory Data Analysis)** ⏱️ 15 minutes
- Visualizations showing churn patterns
- See how age, tenure, geography affect churn
- **Output**: 4 visualization plots + insights

### **SECTION 5: Feature Engineering** ⏱️ 10 minutes
- Create new features (Age_Group, Balance_to_Salary_Ratio, etc.)
- **Why?** These help the model learn better
- **Output**: Enhanced feature set

### **SECTION 6: Data Splitting & Scaling** ⏱️ 5 minutes
- Split into training (80%) and test (20%) data
- Scale features to same range
- **Why?** Prevent data leakage, improve model performance

### **SECTION 7: Model Training** ⏱️ 5-10 minutes
- Train 2 models: Logistic Regression & Random Forest
- **Output**: Trained models ready for prediction

### **SECTION 8: Model Evaluation** ⏱️ 10 minutes
- Evaluate both models with multiple metrics
- Compare performance with ROC curves
- See feature importance
- **Output**: Performance metrics and visualizations

### **SECTION 9: Business Interpretation** ⏱️ 10 minutes
- Translate ML results into business insights
- Identify high-risk customers
- Calculate financial impact
- **Output**: Actionable business recommendations

### **SECTION 10: Conclusion** ⏱️ 5 minutes
- Summary of what you learned
- Next steps for production
- **Output**: Project completion summary

---

## Step 5: Expected Output

As you run each section, you should see:

✅ **Console Output**:
```
✅ All libraries imported successfully!
✅ Dataset loaded successfully!
✅ No missing values found
✅ Data Cleaning complete
✅ Visualization 1 created
... and more
```

✅ **Visualizations** (plots will appear):
1. Churn Distribution chart
2. Age vs Churn histogram
3. Geography vs Churn bar chart
4. Tenure vs Churn histogram
5. Correlation heatmap
6. ROC curve comparison
7. Feature importance chart

✅ **Metrics** (displayed as text):
```
Accuracy:  0.8612 (86.12%)
Precision: 0.8525
Recall:    0.8475
F1-Score:  0.8500
ROC-AUC:   0.8923
```

---

## Step 6: Understand the Insights

### Key Findings You'll See:

1. **Churn Rate**: ~20% of customers churn
2. **Age Effect**: Older customers churn more (45 vs 37 years average)
3. **Tenure Effect**: New customers churn more (2.9 vs 5.1 years)
4. **Geography**: Germany has 32% churn rate (vs 16% in France)
5. **Best Model**: Random Forest (86% accuracy, 85% recall)

---

## Step 7: Save Your Work

### Option A: Keep in Jupyter (Local)
- All cells run, but not version controlled
- Good for learning/experimentation
- Easy to share if you convert to PDF/HTML

### Option B: Push to GitHub (Recommended for Portfolio)

```bash
# Initialize Git (one time)
git init
git add .
git commit -m "Day 1: Bank Churn Prediction - Initial commit"

# Connect to GitHub
git remote add origin https://github.com/YOUR-USERNAME/bank-churn-prediction.git
git push -u origin main
```

**Steps to create GitHub repo:**
1. Go to https://github.com/new
2. Name it: `bank-churn-prediction`
3. Add description: "Bank Customer Churn Prediction - Day 1 AI Engineer Journey"
4. Make it Public (for portfolio)
5. Click Create Repository
6. Follow the instructions to push your code
## ❓ Troubleshooting

### Issue: "Module not found" error
**Solution**: 
```bash
pip install -r requirements.txt
```
Then restart Jupyter kernel (Kernel → Restart)

### Issue: Dataset download fails
**Solution**: 
1. Manually download from Kaggle
2. Place CSV in project folder
3. Update file path in notebook if needed

### Issue: Visualizations don't appear
**Solution**: 
```bash
pip install --upgrade matplotlib
```

### Issue: Memory error (dataset too large)
**Solution**:
```python
# At start of notebook, add:
import gc
gc.collect()  # Free up memory
```

### Issue: Kernel crashes
**Solution**:
1. Restart kernel (Kernel → Restart)
2. Run cells in order (don't skip)
3. Clear output (Cell → Clear Output → Clear All Output)


## 📚 Learning Resources (While Running)

While running the notebook, you might want to learn more:

- **ROC-AUC**: https://www.youtube.com/watch?v=4jRBRDbJemM
- **Feature Scaling**: https://scikit-learn.org/stable/modules/preprocessing.html
- **Random Forest**: https://en.wikipedia.org/wiki/Random_forest
- **Confusion Matrix**: https://en.wikipedia.org/wiki/Confusion_matrix

## ✅ Success Criteria

You've completed Day 1 successfully when:
- ✅ All notebook sections run without errors
- ✅ You see visualizations in the output
- ✅ You can explain the model metrics
- ✅ You understand the business insights
- ✅ You can answer the 5 interview questions
- ✅ Code is pushed to GitHub (optional)

