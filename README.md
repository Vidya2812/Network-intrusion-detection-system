# Network intrusion detection system

ABSTRACT

Network Intrusion Detection Systems are critical in bolstering an organization's security infrastructure. The goal of our paper is to design and build a specialized intrusion detection system for simulated military scenarios. The solution classifies network accesses using machine learning techniques and seamlessly integrates the Ethereum blockchain for secure anomalous access record-keeping and auditing. The machine learning component classifies the records as normal or anomalous using the ensemble learning technique, which is the random forest classifier. Feature selection techniques like Variance Threshold, Spearman’s correlation coefficient, Pearson’s correlation coefficient, Mutual Information and Chi square tests were used to improve the accuracy of the model and reduce dimensionality. The final accuracy of the model was brought to 96.69%. It then sends the records to the blockchain environment for storage. To ensure data integrity and transparency, anomalous access events will be time-stamped, hashed using IPFS, and published to the blockchain. By providing a hash value and a unique id as input, the user will be able to add new anomalous entries. Furthermore, the user will be able to examine the hashed anomalous data for each csv file using the proper id.

RESULTS AND DISCUSSION 

This is the summary of a machine learning model using Random Forest Classifier.
●	The model built using the variance threshold method gave an accuracy of 99.35% before hyperparameter tuning and 96.54% after hyperparameter tuning. 
●	Similarly the models built using chi square test and pearson’s correlation coefficient gave an accuracy of 99.35% before hyperparameter tuning and 96.2% and 96.1% respectively after hyperparameter tuning. 
●	The ML model, trained on a 19-feature training dataset, achieved an accuracy of 99.35%, overfitting the training dataset after a common subset of features was selected.
●	After hyperparameter tuning the accuracy was fine tuned to 96.69% which is the best obtained accuracy by far after hyperparameter tuning. 

Variance threshold Model Accuracy 

![image](https://github.com/user-attachments/assets/d1c812f2-84ad-4890-ad84-96de158105c6)

Chi square Model Accuracy

![image](https://github.com/user-attachments/assets/49672f8b-15c9-444b-b206-e68df811e167)

Pearson’s correlation coefficient Model Accuracy

![image](https://github.com/user-attachments/assets/4382a50d-108e-416d-bf84-bfeb24930548)

Best subset Model Accuracy 

![image](https://github.com/user-attachments/assets/e17bb401-f219-4e4f-a9cb-55f9bade6398)

CONCLUSION

The experimental network accesses were gathered, and various machine learning methods were applied to build an efficient machine learning model. The model was trained on the meaningful characteristics by filter-based feature selection techniques such as statistical filter-based approaches, variance threshold analysis, and correlation coefficient. This involved in determining whether a network access is normal or anomalous and storing the anomalous attacks using blockchain. Storage of anomalous attacks in a decentralized and distributed network is achieved by the usage of blockchain technology which will serve as a repository for historical data for anomalous attacks.  Future research in multi class classification can be used to analyze the data stored in existing blockchain network and predict the exact type of anomalous access such as phishing, denial of service, malware, DNS attacks etc.


