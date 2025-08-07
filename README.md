💳 Fraud Detection in Financial Transactions

This project implements a machine learning-based system for detecting fraudulent financial transactions using PySpark on AWS EMR. It includes data preprocessing in Hive, model training with Random Forest, and evaluation using ROC-AUC.



 📌 Problem Statement

With the increase in digital transactions, financial fraud has become a significant issue. This project aims to develop a scalable fraud detection pipeline using big data tools.



 🛠 Tools & Technologies

- Apache Spark (PySpark)
- Hive on Cloudera
- AWS EMR & EC2
- Python
- Random Forest Classifier
- Jupyter Notebooks



 📂 Project Structure


fraud-detection-system/
├── data/                   # Dataset used
├── notebooks/              # PySpark notebook
├── results/                # Output files (e.g. model results, ROC curve)
├── report/                 # Final report and project presentation
└── README.md               # Project overview
```



 📊 Dataset

The dataset includes:
- Transaction details (amount, origin, destination)
- Balance before/after transaction
- Fraud indicator labels

Located in: `data/Fraud_detection_system.csv`



 ⚙️ How to Run

1. Set up AWS EMR with Spark and Hive installed.
2. Upload dataset to HDFS or use directly in notebook.
3. Run `notebooks/Spark_Notebook.ipynb` using PySpark Jupyter.
4. Review outputs and ROC results in `results/`.



 🧠 ML Model

- Model: Random Forest Classifier
- Hyperparameter Tuning: Grid Search over `numTrees` and `maxDepth`
- Evaluation Metric: Area Under ROC Curve (AUC-ROC)



 👥 Team Members

- Sathwika Karingu (Team Lead): AWS + EMR Setup, Notebook, Report
- Krishna Anuhya Regalla: Data Visualization
- Vivek Nelluri: Hive-based SQL preprocessing
- Hari Krishna Sai Rachuri: Model development and hyperparameter tuning



 📈 Result

Achieved AUC = 1.0, indicating a perfect classifier on the validation set.



 📎 References

- [Real-time Financial Fraud Detection using Big Data](https://example.com)
- "Fraud Detection in Hadoop Ecosystem" – Procedia CS, 2017