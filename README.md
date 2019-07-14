# Fraud_detection_simple
Simple solution for Fraud detection problem.
# Data
* "Fraud_Data": information about each user first transaction.
* "IpAddress_to_Country": mapping each numeric ip address to its country. For each country, it gives a range. If the numeric ip address falls within the range, then the ip address belongs to the corresponding country.
# Columns in Fraud_Data:
* user_id: ID of the user. Unique by user
* signup_time: the time when the user created his/her account (GMT time)
* purchase_time: the time when user bought the item (GMT time)
* device_id: the device id. You can assume that it is unique by device. I.e, 2 transactions with the same ID means that the same physical device was used to buy.
* source: user marketing channel: ads, SEO, Direct (i.e. came to the site by dicrectly typing the site address on the browers)
* browser: the browser used to by the user
* sex: user sex (Male or Female)
* age: user age
* ip_address: user numeric ip address
* class: this is what we are trying to predict: whether the activity was fraudulent (1) or not (2).
# Coulumns in IpAddress_to_Country:
* lower_bound_ip_address: the lower bound of numeric ip address for that country.
* upper_bound_ip_address: the upper bound of numeric ip address for that country.
* country: the corresponding country. If a user has an ip address whose value is within the upper and lower bound, then he/she is based in this country

# Model
* As you can see in my solution, this is imbalance dataset. Intuitively, we should use roc_curve metric. I tryed to train with 3 model: kNN, random forest and decision tree.


** Star if you like:)
