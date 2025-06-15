# Predicting-Offer-Retraction-by-Candidates-in-IT-Hiring-using-Logistic-Regression
Predictive modeling to identify candidates likely to retract accepted job offers using logistic regression with class weighting and threshold tuning.



# Predicting Offer Retraction by Candidates in IT Hiring using Logistic Regression

 Project Overview
This project addresses a critical HR problem in the Indian IT services industry — candidates who **accept job offers but later retract**. Using historical hiring data, we build a logistic regression model that predicts the likelihood of offer retraction, helping HR teams reduce wasted time, cost, and resource planning issues.

This problem is based on a real-world case study from **ScaleneWorks**, a recruitment consulting firm helping IT companies streamline their talent acquisition processes.

---

 Problem Statement
- **Business Impact**: When candidates retract offers late in the recruitment cycle, companies are forced to restart hiring, resulting in productivity and financial losses.
- **Goal**: Predict whether a candidate will **join (1)** or **retract their offer (0)**.
- **Challenge**: The dataset is highly imbalanced — most candidates join, while only a few retract.

---

Methodology
1. **Data Cleaning & Feature Engineering**
   - Processed categorical and numeric features
   - Created derived variables like "difference between expected vs offered CTC"

2. **Modeling Approach**
   - Used Logistic Regression with `class_weight='balanced'` to account for class imbalance
   - Tuned the classification threshold to increase sensitivity to offer retractions

3. **Evaluation Metrics**
   - Confusion Matrix, Precision, Recall, F1-score
   - ROC Curve and AUC to help choose a business-relevant threshold

---

 Results
- Significant improvement in recall for candidates likely to retract offers
- AUC and ROC curve analysis helped identify better decision thresholds
- Model aligned more closely with business priorities: avoiding last-minute retractions

---

 Key Learnings
- Imbalanced datasets can mislead model performance metrics like accuracy
- For business-critical minority classes, **recall matters more than precision**
- Logistic Regression, combined with proper weighting and threshold tuning, is a strong baseline model



