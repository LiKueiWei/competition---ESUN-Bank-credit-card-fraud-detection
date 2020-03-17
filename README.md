# competition---ESUN-Bank-credit-card-fraud-detection

**This challenge was held during Sep 2019 to Nov 2019.**  
**I didn't join the competition but got the dataset accidently.**  
**So here shows what I've tried to make the model F1-score over 0.9.**  


**Method**  
* (1) Selected features: cano, locdt, fraud_ind, scity, mchno, loctm, etymd, ecfg, conam, csmcu, flg_3dsmk, ovrlt, contp, flbmk, hcefg, insfg, iterm, mcc, stocn, stscd  
* (2) Created features: sus_loctm, sus_city, sus_etymd, sus_csmcu, sus_locdt, tm_3ds_ovr_ecfg, ovrlt_ecfg, sus, fraud_conam, sus_sus_loctm
* (3) Model: Random Forest  


**Score**  
higest F1-score = 0.9386 (Top 1%)  
Accuracy = 0.9989  
Precision = 0.9667  
Recall = 0.9121  
Average running time = 120 seconds  

`The codes are shown in another jupyter notebook`  

**Dependencies**  
Python 3.7  
pandas  
sklearn  
pyecharts  
seaborn  
numpy  
matplotlib.pyplot  
