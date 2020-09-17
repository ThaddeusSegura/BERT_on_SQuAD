# BERT Self-Ensemble Methods on SQuAD v2.0

<br/>
This repo contains a number of files relating to an exploration of Self-Ensemble methods using BERT on SQuAD v2.0.<br/>

I would recommend viewing the file w266_final first, as it is a presentation which explains the overall approach.<br/>

The file thaddeus_segura_w266 is a paper explaining the process more formally.<br/>

Then I would move on to the relevant files you would like to explore.  All of these are notebooks as they were run in Colab, some using TPU's and others on GPU's. <br/>

### Files 
<br/>
--EDA---<br/>
1) squad_eda.ipynb: This is the notebook containing the EDA of the SQuAD v2.0 Dataset<br/>
<br/>
---BASELINE---<br/>
2) Baseline.ipynb: This contains the baseline model<br/>
<br/>
---DISCRETE DATA PRESENTATION---<br/>
3) Self_ensemble_4.ipynb: 4 way split and training of the dataset.<br/>
4) Self_ensemble_8.ipynb: 8 way split and training of the dataset. <br/>
<br/>
---DNN FOR MODEL SLECTION---<br/>
5) SE_8_pred_and_label.ipynb: used to generate data that was used to train the multiple choice model and the deep neural net model.<br/>
6) Deep_ensemble_8.ipynb: the model that was trained to select the best model for each question.<br/>
<br/>
---MULTIPLE CHOICE---<br/>
7) SE1_generate_data.ipynb: generation of data for multiple choice based on a self ensemble using different splits of the data. <br/>
8) SE4_generate_data.ipynb:  generation of data for multiple choice based on 4 way split.<br/>
9) SE1_multi_choice.ipynb:  This used the top 4 predictions plus the null prediction with a Bert for multiple choice model.<br/>
10) SE4_multi_choice.ipynb: Same as SE1 but with a different dataset.<br/>
11) SE4_AB.ipynb:  This reduced the number of predictions from 5 to 2, applied only to the 4 way split.<br/>
<br/>
---CLASSIFICATION---<br/>
12) SE_classification.ipynb: train a classifier to predict the answerable/unanswerable questions and use this to overwrite the other predictions.<br/>
<br/>
---INTELLIGENT WEIGHTING---<br/>
13) intelligent_voting.ipynb: Combining the previous models using model confidence, callibration, and fine-tuning.<br/>
<br/>
---REPORT---<br/>
14) thaddeus_segura_w266.pdf: The write up of the findings.<br/>
<br/>
---SLIDES---<br/>
15) w266_final.pdf: The slides outlining the findings.<br/>
