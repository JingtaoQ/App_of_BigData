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
  
        shap.plots.beeswarm(shap_values)

    </html>   

  ![Visualize1](https://github.com/JingtaoQ/App_of_BigData/blob/main/pic/p3-1.png "Visualize1")
    
- Visualize explanations for all points of  your data set at once
    <html>

        ind = 0
        shap.plots.force(shap_values[ind],matplotlib=True)

    </html>
  
  ![Visualize2](https://github.com/JingtaoQ/App_of_BigData/blob/main/pic/P3-2.png "Visualize2")
- Visualize a summary plot for each class on the whole dataset
    <html>

        shap.summary_plot(train, test, plot_type="bar",feature_names=features)

    </html>

  ![Visualize3](https://github.com/JingtaoQ/App_of_BigData/blob/main/pic/P3-3.png "Visualize3")