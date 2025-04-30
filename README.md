# SCADA Predictive Maintenance Project

This repository contains an end-to-end machine learning pipeline simulating predictive maintenance for SCADA-style sensor data. It was developed in alignment with the Certarus Summer Co-op (AI/ML) position and demonstrates the full lifecycle of a failure prediction system up to model training and evaluation.

## Project Overview
The project uses synthetic sensor data to predict potential equipment failures using classification models. It includes:
- Data ingestion from PostgreSQL
- Cleaning and preprocessing
- Model training and evaluation

## Key Features
- **Sensor Data:** `temperature`, `pressure`, `vibration`, and binary `failure_flag`
- **Database:** PostgreSQL (created using pgAdmin4, queried via SQLAlchemy)
- **Missing Value Handling:** Interpolation and forward-fill
- **Outlier Detection:** IQR-based filtering
- **Model:** Random Forest (scikit-learn)
- **Evaluation Metrics:** Precision, Recall, F1-score, Confusion Matrix

## Technologies Used
- Python 3.9
- pandas, NumPy, scikit-learn
- PostgreSQL, SQLAlchemy
- Jupyter / Google Colab

## Notebook
- [`scada_portfolio_project.ipynb`](https://github.com/ramneeth/SCADA_Project/blob/main/scada_portfolio_project.ipynb)

## Folder Structure (planned)
```
SCADA_Project/
├── scada_portfolio_project.ipynb     # Main notebook
├── data/
│   └── noisy_scada_data.csv          # Simulated SCADA dataset
├── README.md                         # Project overview
```

## Real-World Relevance
This project reflects Certarus's goals of reducing downtime and improving safety through AI and real-time sensor analysis. It was built to mirror a production environment using open-source tools and practical, deployable ML design principles.

## Future Improvements
- Add time-based feature engineering (rolling stats, lag features)
- Extend to Azure ML and Event Hub for cloud-based deployment
- Integrate with Databricks for large-scale time-series data handling

---

**Author:** Ramneet Hunjan  
**GitHub:** [@ramneeth](https://github.com/ramneeth)

