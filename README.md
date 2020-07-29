# w266_final
Final Project Repo for w266

This repo contains a number of files for the final project for w266.
These were all run via colab to make use of GPU's and TPU's.

--EDA---
1) squad_eda.ipynb: This is the notebook containing the EDA of the SQuAD v2.0 Dataset

---BASELINE---
2) Baseline.ipynb: This contains the baseline model

---DISCRETE DATA PRESENTATION---
3) Self_ensemble_4.ipynb: 4 way split and training of the dataset.
4) Self_ensemble_8.ipynb: 8 way split and training of the dataset. 

---DNN FOR MODEL SLECTION---
5) SE_8_pred_and_label.ipynb: used to generate data that was used to train the multiple choice model and the deep neural net model.
6) Deep_ensemble_8.ipynb: the model that was trained to select the best model for each question.

---MULTIPLE CHOICE---
7)SE1_generate_data.ipynb: generation of data for multiple choice based on a self ensemble using different splits of the data. 
8)SE4_generate_data.ipynb:  generation of data for multiple choice based on 4 way split.
9)SE1_multi_choice.ipynb:  This used the top 4 predictions plus the null prediction with a Bert for multiple choice model.
10)SE4_multi_choice.ipynb: Same as SE1 but with a different dataset.
11)SE4_AB.ipynb:  This reduced the number of predictions from 5 to 2, applied only to the 4 way split.

---CLASSIFICATION---
12)SE_classification.ipynb: train a classifier to predict the answerable/unanswerable questions and use this to overwrite the other predictions.

---INTELLIGENT WEIGHTING---
13)intelligent_voting.ipynb: Combining the previous models using model confidence, callibration, and fine-tuning.

---REPORT---
14)thaddeus_segura_w266.pdf: The write up of the findings.

---SLIDES---
15)w266_final.pdf: The slides outlining the findings.
