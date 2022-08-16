# Toxicity-Prediction
What is toxicity and soureces of it:
      Toxicity – The adverse effects that a chemical may produce.
      Source – Drugs, Pesticides, Natural toxins, Pollutants, Hazardous chemicals etc.,

Objective:
      To build a robust model using Machine Learning for toxicity prediction.
      Identify the fragments common to both toxic and non-toxic compounds.
  
Dataset: 
  Dataset were collected from databases like KEGG-Drug, Drug Bank, TOXNET, T3DB, FDA. 
  
Data Pre-processing:
  Redundant, complex structures and salt compounds were removed in this step.
  
Feature Engineering:
  Original datset size was about 5655(toxic -1) and 5334(non-toxic -0) compounds.
  Undersampling was performed to balance the dataset to 5334(toxic -1) and 5334(non-toxic -0) -- Total 10,668 compunds in total.
  
Molecular Fingerprints:
  The compounds structural fragments are considered based on their presence (i.e, 0 and 1) to vector form.The types of fingerprints considered are MACCS, PubChem, Klekota Roth, Atom Pair 2D.
  
 Machine Learning Models used:
  Random Forest(RF), Support Vector Machine(Linear, RBF, Polynomial)
  
 Model Evaluation & Validation:
  The model was evaluated using various metrics like Accuracy, MCC, Precision, F1-Score. Finally, the model was evaluated using FDA dataset (size- 1566) which was not part of training dataset.
  
Conclusion:
  THe model was able to achieve a validation accuracy between 78%-85% with AUC of 0.75-0.98 of which MACCS outperformed with AUC of 0.98. Developing such predictive models can be helpful in toxicity prediction of a new drug candidate in the drug discovery pipeline.
