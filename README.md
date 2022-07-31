# machine-learning-classification-covid19
### Comparision between machine learning models in the classification of death by covid-19

The following project I used for my final paper in college. 


The Scikit-Learn library along Jupyter Notebooks made in Python, was used for all models for classification. 

The dataset was provided by the state of São Paulo in the website https://www.seade.gov.br/coronavirus/.
This dataset has all confirmed cases with the covid-19 in the state of São Paulo, and is being updated day by day until the publication of this project.
I used because has columns with various comorbidities and others important datas to apply the study, like age, death and gender. Some columns I droped manually.
The sampling period is between 04/02/20 to 21/03/21.

Columns used:
- idade (age)
- cs_sexo (gender)
- obito (death)
- asma (asthma)
- cardiopatia (heart disease)
- diabetes
- doenca_hematologica (hematological disease)
- doenca_hepatica (liver disease)
- doenca_neurologica (neurological disease)
- doenca_renal (kidney disease)
- imunodepressao (immunosuppression)
- obesidade (obesity)
- outros_fatores_de_risco (other risk factors)
- pneumopatia (lung disease)
- puerpera (puerperal)
- sindrome_de_down (Down's syndrome)

After the proper treatment of the dataset, a transformation was made in the data for numerical values using Label Encoder fuction. 
The variable target was death with values 0 and 1, but before the balance of the samples, the dataset has more than 97% to value 0. 
Because the unbalanced, were used the Imblearn library with the under sampling method, equaling the samples category values, but losing much data.

The models were made are Decision Tree, Random Forest, SVM with linear and rbf kernel and Neural Networks of multilayer perceptrons, with adam and lbfgs solver.

After the separation of samples between training and test datasets in the 70/30 proportion, were used metrics to attest to the learning of the models.
