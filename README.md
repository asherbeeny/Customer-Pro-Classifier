# Customer-Pro-Classifier
 
# Quick Observations
- hash_trans_id : Not unique, one transaction has multiple records under it
- sku_id: can be split into 2 parts to be used in the classification
- online_order_type: always = "IN-STORE" then can be droppped.
- online_order_type_desc : always = "IN-STORE" then can be droppped.
- transaction_type : many Refund/returns transaction types that need to be handled/dropped
- transaction_sales_type: many returns transaction types that need to be handled/dropped
- pos_sales: min & max values looks like outliars and negative values need to be explored and cleaned.
- pos_unitssold:min & max values looks like outliars and negative values need to be explored and cleaned.
- department_id: can be used in the model as is with opportunity to be used as one-hot encoded features
- class_id: can be used in the model as is with opportunity to be used as one-hot encoded features
- subclass_desc : text features need to be extracted from this column with opporunity to be used in product classification
- product_weight:Products with 0 weight need to be explored, can be used as normalized feature
- product_weight_dimension: can be used as one-hot encoded features
- product_height: Products with 0 and max height need to be explored, can be used as normalized feature
- product_length : Products with 0 and max length need to be explored, can be used as normalized feature
- product_width: Products with 0 and max width need to be explored, can be used as normalized feature
- product_unit_dimension : Products with units value 0 need to be explored, can be used as one-hot encoded features
- product_volumn: Products with 0 and max volume need to be explored, can be used as normalized feature
- product_volumn_unit: Products with units value 0 need to be explored, can be used as one-hot encoded features
- pro: the target variable, balanced distribution, train/test split class distribution need to be verified
- transaction_timestamp : transaction ranges between May 2013 - Dec 2015
- transaction_year: most of the transaction is in 2015
- transaction_month: top transction count is in November and May (beining of Summer season and begining of winter season)
- transaction_day: good distribution across days of the month
- transaction_hour: most of the transaciton is in hte morning and noon time
- transaction_weekday: good distribution across days of the week
