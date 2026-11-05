AI-Based Intrusion Detection System

Machine Learning | Cybersecurity | Data Science | Python

Project overview

This project explores the use of machine learning to identify malicious network traffic using the UNSW-NB15 intrusion-detection dataset. The notebook covers data preparation, classification, comparison of model performance, and evaluation of the challenges involved in detecting different types of network attacks.

The work includes both binary classification (normal versus attack traffic) and multi-class classification (distinguishing attack categories).
Key results
Binary classification
Model	Reported accuracy
Random Forest	98.48%
K-Nearest Neighbours (KNN)	98.16%
Decision Tree	97.92%


Random Forest achieved the highest reported binary-classification accuracy among the models compared.
Multi-class classification
The Random Forest multi-class model achieved approximately 88.72% accuracy, with a macro F1-score of approximately 0.40. The difference between accuracy and macro F1-score indicates that performance was uneven across classes, especially for less frequent attack categories.
Interpretation note: These numbers reflect saved outputs in the project notebook, not independently reproduced results or a validated production deployment. Some preprocessing steps (including scaling and correlation-based feature selection) were applied before the train/test split. Future work should fit all learned preprocessing steps on training data only and re-evaluate performance to reduce the risk of data leakage.

Workflow
1. Data preparation: Examined and prepared network-traffic data for modelling.
2. Preprocessing: Encoded categorical variables and applied feature-preparation techniques.
3. Model development: Trained and compared Random Forest, KNN, and Decision Tree models.
4. Evaluation: Used metrics such as accuracy, precision, recall, F1-score, and confusion matrices to assess results.
5. Analysis: Compared binary and multi-class results, identifying limitations associated with imbalanced classes.
Technologies and tools
- Python and Jupyter Notebook / Google Colab
- Pandas and NumPy
- Scikit-learn
- Machine learning classification and model evaluation
- UNSW-NB15 dataset
Explore the project
- [View the Jupyter Notebook](Intrusion_Detection_Models.ipynb) — code, experiments, and saved outputs.
- [Read the dissertation](A3%20Dissertation.pdf) — detailed project write-up.
- [View the notebook PDF](Intrusion%20Detection%20Models.ipynb%20-%20Colab.pdf) — exported notebook.
Limitations and next steps
- Rebuild preprocessing as a training-only pipeline and run leakage-resistant evaluation.
- Investigate class imbalance and per-class recall in multi-class attack detection.
- Compare performance using additional validation splits or cross-validation.
- Document dataset provenance, exact environment dependencies, and reproducibility instructions.
  
Author

Daniel Akpomon-Daniels

Academic data science and machine-learning portfolio project.
