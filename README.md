## _Safe-to-fly_ : An On-board Intelligent Fault Diagnosis System With AutoML for Unmanned Aerial Vehicles [[Paper](https://ieeexplore.ieee.org/document/9752852) | [Code](https://github.com/RITIK-12/safe-to-fly)]

<img width="1196" alt="Screenshot 2022-09-20 at 11 23 03 AM" src="https://user-images.githubusercontent.com/54806252/191177931-70de6492-6874-4bb0-aa5f-9d82081f55e8.png">

### ✯ Abstract
Real-time fault diagnosis in Unmanned Aerial Vehicles (UAVs) is a challenging task. Data-driven intelligent diagnosis of faults ensures flight safety for UAVs. In this paper, realtime fault diagnosis on small scale fixed-wing UAVs has been shown by data of natural flight conditions with a wrapped wing structure that breaks the geometric symmetry. AutoML based approach was taken for multi-class fault classification. Two datasets were created from the combination of flight data of two days. The experimental results showed that the proposed Deep Learning AutoML model significantly improves performance over conventional Machine Learning methods such as the Decision Tree, KNN, and the Random Forest. The test accuracy of the proposed AutoML model was 74% and 100% on the first and second datasets, respectively. The AutoML model’s capability in classifying low fault severity and complex faults demonstrated the method’s usefulness and excellence.

### ✯ Datset Acquisition & Preparation
* The dataset for the fault detection was acquired from M. Bronz et al. [6]. It contains multi-class fault data for two days(21st of July 2020 and 23rd of July 2020) of identical flights.
* It comprised of faults related to left control surface efficiency and right control surface efficiency with eight fault types and normal flight data.
* Two datasets are created by the combination of flight data for two days. The first dataset consists of the flight data of 21st July, which has been divided into training and testing data with an 80:20 split.
* The second dataset is created by combining flight data of 21st July and 23rd July and dividing the data in training and testing set of split size 80:20.


<img width="1314" alt="Screenshot 2022-09-20 at 12 02 05 PM" src="https://user-images.githubusercontent.com/54806252/191184038-e8e78977-8153-48b5-bfc2-b2ed775170fa.png">

### ✯ Fault Detection Method
* Several state-of-the-art Machine Learning algorithms such as Decision Tree Classifier, KNN, and Random Forest Classifier were applied on the datasets for comparison of the results with the AutoML model.
* Auto-Keras leverages Neural Architecture Search, but with the addition of network morphism and Bayesian optimisation to direct the network morphism for a more effective neural network search. 
* The Safe-to-fly AutoML Model I was trained on flight data of 21st July and tested on 23rd July data. 
* The Safe-to-fly AutoML Model II was trained on 80% of combined data of 21st July and 23rd July and evaluated on the rest 20% data.
<p align="center">
  <img width="500" alt="Screenshot 2022-09-20 at 12 05 02 PM" src="https://user-images.githubusercontent.com/54806252/191184648-913d910a-1ef5-4198-819f-90a8f3c4dc26.png"> 
  <img width="500" alt="Screenshot 2022-09-20 at 12 05 26 PM" src="https://user-images.githubusercontent.com/54806252/191184670-ee35a2de-3a66-4e1d-8c6a-6a058db63497.png">
</p>

### ✯ Model Evaluation on Dataset 1
* Table III shows a comparison of training and test accuracy for different ML Algorithms employed. 
* It is evident that the AutoML model has comparable results with respect to other ML Algorithms.
* The Fig. 3 shows the comparison of different performance metrics, namely Precision, Recall and F-1 Score for the ML models.
* As the testing dataset was of an entirely different flight, the AutoML model performance demonstrates its usability in the real world.

<p align="center">
  <img width="500" alt="Screenshot 2022-09-20 at 12 19 09 PM" src="https://user-images.githubusercontent.com/54806252/191187126-e2523647-18b9-4ad1-9593-de90e93ccec1.png">
  <img width="500" alt="Screenshot 2022-09-20 at 12 19 49 PM" src="https://user-images.githubusercontent.com/54806252/191187169-41dad6f8-34b4-46f1-8640-7f7fe65062cd.png">
</p>

### ✯ Model Evaluation on Dataset 2
* As the Dataset 2 was prepared by combining the flight data of 21st and 23rd July, which resulted in larger training data than the previous case. 
* Hence an improvement in the performance of all the ML Algorithms can be seen.
* The Table IV shows the comparison of different performance metrics values for the various Machine Learning algorithms with the proposed AutoML model. 
* The Fig. 4 shows the Confusion Metrics obtained when the AutoML model was evaluated on the test dataset.
* It is evident from the confusion matrix that AutoML nearly classified all the faults accurately.
* The Fig. 5 shows the comparison of performance metrics for different types of faults, which was obtained with the help of the Confusion Matrix.
* The high values of precision recall and F-1 score shows the efficiency of the AutoML model.
* This also proves the usability and generality of the AutoML model used.

<p align="center">
<img width="300" alt="Screenshot 2022-09-20 at 12 25 13 PM" src="https://user-images.githubusercontent.com/54806252/191188248-5d20b583-1629-4086-a39f-92adee50c645.png">
<img width="300" alt="Screenshot 2022-09-20 at 12 25 40 PM" src="https://user-images.githubusercontent.com/54806252/191188279-e6418233-6b43-4ee8-ae89-f5cb41387756.png">
<img width="300" alt="Screenshot 2022-09-20 at 12 25 52 PM" src="https://user-images.githubusercontent.com/54806252/191188364-08e0cf5a-277c-48d8-adea-fa359d168347.png">
</p>

### ✯ BibTeX
If you find this code or paper useful, please use the following reference:

```
@INPROCEEDINGS{9752852,  
author={Bompilwar, Ritik and Rathor, Surya Pratap Singh and Sinha, Aparna and Das, Debanjan},  
booktitle={2022 IEEE Delhi Section Conference (DELCON)},   
title={Safe-to-fly : An On-board Intelligent Fault Diagnosis S<img width="639" alt="Screenshot 2022-09-20 at 12 25 52 PM" src="https://user-images.githubusercontent.com/54806252/191188314-cb1cd52f-d932-4426-bb8d-4b51cad6ae33.png">
ystem With AutoML for Unmanned Aerial Vehicles},   
year={2022},  
volume={},  
number={},  
pages={1-5},  
doi={10.1109/DELCON54057.2022.9752852}}
```

### ✯ References
1. https://www.kaggle.com/datasets/sujaradha/thermal-images-diseased-healthy-leaves-paddy
