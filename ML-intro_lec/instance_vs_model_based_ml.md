# Classical ML Algorithms: Instance-Based vs Model-Based Learning

## Key Idea

| Aspect | Instance-Based Learning | Model-Based Learning |
|---|---|---|
| Core idea | Store training data (or most of it) and compare new data to it at prediction time | Learn a general function/parameters from training data, then discard the data |
| Learning phase | "Lazy" — little to no work done upfront | "Eager" — does the work upfront to fit a model |
| Prediction phase | Slow (needs to search/compare against stored data) | Fast (just plug into learned function) |
| Memory usage | High (must keep training data) | Low (only keeps learned parameters) |
| Generalization | Via similarity/distance to known examples | Via a fitted mathematical function |

## Classification Table

| Algorithm | Type | Notes |
|---|---|---|
| k-Nearest Neighbors (k-NN) | Instance-Based | Classic example; predicts via distance to k closest points |
| Locally Weighted Regression (LWR) | Instance-Based | Fits a local model per query point using nearby data |
| Case-Based Reasoning | Instance-Based | Solves new problems using stored similar past cases |
| Radial Basis Function Networks (RBFN) | Instance-Based (partly) | Uses distance from stored/prototype centers |
| Linear Regression | Model-Based | Learns fixed coefficients (weights) |
| Logistic Regression | Model-Based | Learns fixed coefficients for a decision boundary |
| Naive Bayes | Model-Based | Learns probability distributions/parameters from data |
| Decision Trees | Model-Based | Learns a fixed tree structure of rules |
| Random Forest | Model-Based | Ensemble of learned decision trees |
| Gradient Boosting (XGBoost, LightGBM, etc.) | Model-Based | Learns an additive ensemble of weak models |
| Support Vector Machines (SVM) | Model-Based | Learns a fixed separating hyperplane (support vectors define it, but prediction uses the learned boundary, not raw comparison to all data) |
| Neural Networks / Perceptron | Model-Based | Learns fixed weights via optimization |
| K-Means Clustering | Model-Based | Learns fixed cluster centroids |
| Linear Discriminant Analysis (LDA) | Model-Based | Learns fixed projection/decision parameters |

## Quick Rule of Thumb
- **Instance-based** → "memorize and compare" (needs training data at prediction time)
- **Model-based** → "learn and generalize" (training data can be discarded after fitting)
