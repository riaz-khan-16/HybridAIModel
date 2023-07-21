
# Autoencoders ML_Classifier Hybrid Machine Learning Model

This section provides the outcomes of using machine learning models to categorize transformers into excellent, good, medium, bad, or extremely poor categories. SVM, Logistic Regression, Decision Tree, and Random Forest classifiers are trained with the dataset for this purpose. The ML classifier has low classification performance due to a large number of input characteristics (31) and the limited amount of data (607) used. Dimension reduction is required to solve this issue. Therefore, feature extraction and dataset compression are both done using autoencoders. The autoencoder produces a compressed dataset, which is then used by ML classifiers for classification. This section details the performance of various model types, environment setup, and dataset preparation.

![architecture](https://github.com/riaz-khan-16/Autoencoders_with_ML_Classifier/assets/63443462/0bc57268-8947-42a5-8ed5-37198fc45f06)

### Training Dataset Analysis:

The class of transformer is determined using 32 input parameters. Ten different types of transformers are represented in the training dataset: Three categories: good level-1, good level-2, and good level-3—are used to categorize good transformers. The optimum condition is at good level-1, whereas good level-2 is superior to good level 3. Moderate-1, moderate-2, moderate-3, and moderate-4 are the four classes into which medium-type transformers are separated. Compared to moderate-2, moderate-3, and moderate-4, moderate-1 implies better condition. Similar to that moderate-3 is a better condition than moderate-4. Moderate-2 indicates a better state than moderate-3. The three classifications of poor transformers are poor level-1, poor level-2, and poor level-3. There is a total of 10 classes and their statistics are shown in the  table.

![image](https://github.com/riaz-khan-16/Autoencoders_with_ML_Classifier/assets/63443462/9c18e2d5-6557-4399-b69a-52bebf15e1f9)


### Environment Setup

In this experiment total of 8 models are implemented and evaluated. In the algorithmic implementation, the Google Colaboratory software package has been used with the necessary modification and extension. In the experiment, the original database of 607 records is randomly split into two parts of a training dataset and a testing dataset for validating the classification accuracy of the above eight algorithms, where 70% of samples of the original dataset are considered for the training dataset and the remaining 30% for the testing dataset. It is worth pointing out that the data is scaled to [-1, 1] interval before running any algorithm. The above dataset split, cross-validation, and testing will be repeated 100 times for every algorithm.


![image](https://github.com/riaz-khan-16/Autoencoders_with_ML_Classifier/assets/63443462/f473a670-48f0-4cf4-a728-e42e29d872bb)



### Implementing ML Classifier in the compressed dataset

The machine learning classifiers' classification outcomes weren't adequate for the task. However, because a transformer is a crucial component in the transmission and conversion of electricity, it is required to forecast the real class of a transformer. Therefore, feature extraction was carried out using various autoencoder types in order to produce reliable prediction results, and the new dataset that was mentioned in the previous study was developed. . The compressed dataset was then classified using machine learning classifiers. As a consequence, integrated models are developed, and these models produce excellent classification outcomes. Figure [] displays each autoencoder's representation of the classification results using a confusion matrix for the logistic regression classifier. The combined MLPA/Logistic Regression model produces the best results overall in terms of classification accuracy. The classification accuracy of the combined model made with MLPA and Logistic Regression gives the best results among all the models.



![image](https://github.com/riaz-khan-16/Autoencoders_with_ML_Classifier/assets/63443462/184288eb-9c63-4c4c-a52e-d93cbea3d2d8)












![confusion_matrix](https://github.com/riaz-khan-16/Autoencoders_with_ML_Classifier/assets/63443462/50532fdb-e64d-4738-89dc-3c67f3668519)



![heat_map](https://github.com/riaz-khan-16/Autoencoders_with_ML_Classifier/assets/63443462/4ccfeab6-b41d-493d-a7d3-58bb269fd685)


![loss_curve](https://github.com/riaz-khan-16/Autoencoders_with_ML_Classifier/assets/63443462/99603bcd-f7bf-4014-84b1-a7853bcbf2ba)


![result_table](https://github.com/riaz-khan-16/Autoencoders_with_ML_Classifier/assets/63443462/fda48c80-8bcc-4e2b-9cfa-519cb6f4b0d5)
