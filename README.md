# MLflow Porjet - (Home Credit Risk Classification + MLflow + SHAP)
## Home Credit Risk Classification
- Pre-Operation
- LogisticRegression
- Predictions
- Propose a solution to Schedule  your ML pipeline
## MLflow
- Integration
- Reusable and Reproducible
- MLflow UI

## SHAP
- Build a TreeExplainer and compute Shaplay Values
    <html>
      
        explainer = shap.Explainer(log_reg, train, feature_names=features)
        shap_values = explainer(test)
      
    </html>

- Visualize explanations for a specific point of your data set

    <html>
        shap.plots.beeswarm(shap_values)<br>
    </html>
  
    <html>
        <img src="https://github.com/JingtaoQ/App_of_BigData/blob/main/pic/p3-1.png">
    </html>
    
- Visualize explanations for all points of  your data set at once
- Visualize a summary plot for each class on the whole dataset