## Traffic Accident Severity Prediction Using Decision Trees

### Project Overview
This project applies **Decision Trees** inside **Altair RapidMiner Studio** to predict traffic accident severity (`Accident_Severity`). The workflow covers a full data pipeline, including target filtering, duplicate removal, mean/mode missing value imputation, and nominal feature engineering, evaluated using a robust **10-fold cross-validation** architecture. 

Across three hyperparameter tuning trials, the models performed as follows:
* **Trial 1 (Baseline):** 51.65% accuracy
* **Trial 2 (Conservative/Pruned):** 50.34% accuracy
* **Trial 3 (Deep/Complex):** 52.16% accuracy

---

### Conclusion
**Trial 3** achieved the highest overall predictive accuracy at **52.16%** because its expanded depth (20) and small minimal leaf size (1 or 2) allowed the tree to map intricate environmental and situational patterns in the data. Conversely, **Trial 2** performed the worst (**50.34%**) because its strict pre-pruning configurations oversimplified the model structure, forcing it to lose its discriminative edge and default to predicting the majority class ("Low" severity) for the dataset.

#### Author: Ngan Nguyen
