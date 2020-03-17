# T-Brain competition---ESUN-Bank-credit-card-fraud-detection

This challenge was held during Sep 2019 to Nov 2019.  
I didn't join the competition but got the dataset accidently.  
So here shows what I've tried to make the model F1-score over 0.9.  

# Method  
* (1) Selected features: cano, locdt, fraud_ind, scity, mchno, loctm, etymd, ecfg, conam, csmcu, flg_3dsmk, ovrlt, contp, flbmk, hcefg, insfg, iterm, mcc, stocn, stscd  
* (2) Created features: sus_loctm, sus_city, sus_etymd, sus_csmcu, sus_locdt, tm_3ds_ovr_ecfg, ovrlt_ecfg, sus, fraud_conam, sus_sus_loctm
* (3) Model: Random Forest  
* (4) Traning:Testing ratio: 78%：22%(1,191,609：330,178)  

# Modeling Skills
* Fraud transaction time usually happens during 23:00 ~ 07:00.  
* Most fraud transactions are online (with or without 3DS or overlap notes).  
* All the fraud transaction amounts are under NTD 3500.  
* Most fraud transaction methods are not changed over time.  
* Most fraud transaction happends within 4 days, or suddenly happens 10 7 days after normal transactions.  
* Transactions that have fixed city, store, currency, etc usually are fraud deals.

# Results  
higest F1-score = 0.9386 (Top 1%)  
Accuracy = 0.9989  
Precision = 0.9667  
Recall = 0.9121  
Average running time = 120 seconds  

              precision    recall  f1-score   support  
  
           0       1.00      1.00      1.00    327061  
           1       0.97      0.91      0.94      3117  
  
    accuracy                           1.00    330178  
    macro avg      0.98      0.96      0.97    330178  
    weighted avg   1.00      1.00      1.00    330178
   
  
'''
        confusion matrix  
             predicted label
|True label  | 0           |    1  |
| 0          | 1           | 0.0003|
| 1          | 0.088       | 0.91 |


'''

`The codes are shown in another jupyter notebook`  



# Dependencies  
Python 3.7  
pandas  
sklearn  
pyecharts  
seaborn  
numpy  
matplotlib.pyplot  



