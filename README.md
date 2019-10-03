This project aims to build a machine learning algorithm for predicting whether customers visiting Google's Merchandise Store will make a purchase in the next 7 days.
Contributed by: Lim Si Ling Evelyn, Lee Meng Yong, Jiang Nan, Desmond Ho
Pls contact nan.jiang.2018@mitb.smu.edu.sg for any questions.

Data:
Google Merchandise Store clickstream data from Google Bigquery from 1 November 2016 to 30 July 2017.

Dataset was extracted by incorporating SQL queries into the Python codes in Google Colab - See Data_Extraction_and_Exploratory_Data_Analysis.ipynb under codes folder. https://bigquery.cloud.google.com/table/bigquery-public-data:google_analytics_sample.ga_sessions_20170801

Training Dataset:
Data\test_dataset.csv

Testing Dataset:
Data\train_validation_dataset.csv
Note: Target variable (transaction) is highly imbalanced with only 3.9% of the non-bounce sessions making a transaction.

Performance Metric: 
F2-score. F2-score considers both precision and recall in the measurement, but implicit computation will give a higher weightage to recall measure, i.e. the ability for the model to be able to capture as many potential customers as possible.

Models:
Random Forest using data w/o any LDA feature engineering and w/o PCA obtained the highest F2-score for the test data out of all the combinations tried.

Best model
Codes\Models without LDA _ PCA.ipynb
Other models
Codes\Models with LDA.ipynb
Codes\Models with PCA.ipynb
Codes\Models without LDA _ PCA with undersampling.ipynb

Report:
Our full report can be found in: 'Project Report.docx'
