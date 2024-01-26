# $${\color{blue}Detection \space \color{blue}of \space \color{blue}Botnet \space \color{blue}{Attacks}}$$	

## Utilizing Machine Learning for the Detection of Botnet Attacks Targeting IoT Devices
You can find the full report for this project at the following link:
https://drive.google.com/file/d/16oCc9ZhtIP3tYDeGMo4JPjaBM4P50G6f/view?usp=sharing
### Project Introduction

#### 1.1 Project Objective
The project aims to design a system capable of real-time detection and classification of IoT botnet attacks, such as Distributed Denial of Service (DDoS), on IoT networks using machine learning and deep learning algorithms.
#### 1.2 Project Description
The project provides insights into the types and structures of IoT botnets, their construction, communication, and the attacks they perform on IoT. It also reviews the latest research in intrusion detection systems that rely on artificial intelligence algorithms for detecting attacks on networks in general and IoT networks specifically. The outcome of this study is a system capable of detecting IoT botnet attacks in real-time, along with studying and developing methods to protect against these attacks.
#### 1.3 Work Steps
1.	Familiarize with programming tools (Python language, Jupyter notebook, Wireshark tools).
2.	Study references to select the test and training dataset.
3.	Study references on machine learning and deep learning algorithms applied to detect attacks on IoT networks.
4.	Propose a detection model based on the completed literature review.
5.	Pre-process the data in the training and test set to extract features.
6.	Prepare the data for input to the model (Data cleaning).
7.	Select the most impactful features (Feature Importance).
8.	Choose machine learning algorithms based on the completed literature review.
9.	Test the algorithms and adopt evaluation metrics, then compare them to choose the best scenario.
10.	Compare the final results with previous findings referenced in the literature.
#### 1.4 Project Flowchart
Figure (1-1) shows the proposed model flowchart. After conducting the literature review, we proposed a model for detection based on a test and training set containing features at the packet level (Packet-based dataset) derived from the selected IoT-23 dataset. The proposed model achieves real-time attack detection and performs multiclass classification of attacks within the training and test set. During the model development, we used three machine learning algorithms: Random Forest, K-Nearest Neighbor, and XGBoost, along with the deep learning algorithm Long Short-Term Memory (LSTM). We compared them based on several criteria and selected the algorithm that provided the best detection accuracy. The flowchart consists of three main sections:
•	Section 1 (Data Pre-processing): Extracting features from the IoT-23 training and test set at the packet level and preparing the data for input to the classifier model.
•	Section 2 (Feature Selection): Choosing the most impactful features.
•	Section 3 (Classifiers Modeling): Implementing machine learning algorithms discussed earlier to select the best algorithm and scenario for optimal real-time attack detection.
 ![image](https://github.com/HindForIot/Detection-of-Botnet-Attacks-Targeting-IoT-Devices/assets/144903433/df3e001d-77cc-42bc-99ec-b245797f0f49)

                                                Figure (1-1): Project Flowchart.





-----------------------------------------------------------------------------------------------------------------------------------------------------------

$${\color{red}It \space \color{red}is \space \color{red}recommended \space \color{red}to \space \color{red}begin \space \color{red}by \space \color{red}reading \space \color{red}the \space \color{red}directories \space \color{red}in \space \color{red}the \space \color{red}order \space \color{red}provided \space \color{red}{here.}}$$

-----------------------------------------------------------------------------------------------------------------------------------------------------------




              
## First Subdirectory: Data-Preprocessing
This subdirectory contains codes implemented for executing the initial processing operation. The purpose of this process is to extract features at the packet level and add attack names corresponding to each packet group. Subsequently, the data is cleaned to prepare it for entry into the classifier model.

Process Input: IoT-23 Dataset (Flow-based dataset)

Process Output: Npacket.csv file (Packet-based dataset)

## Second Subdirectory: Experiments
This subdirectory contains the classifier model applied to the derived dataset, following experiments that include the following:

Application of four algorithms:

1- Random forest.
2- XGBoost.
3- LSTM.
4- KNN.

All these algorithms are implemented for the following cases:
N=1, N=2,..., N=5, N=10, N=15, N=20

N: Number of packets from each flow.

The execution was also conducted based on two scenarios:

Scenario 1: With port numbers.

Scenario 2: Without port numbers.

Process Input: Npacket.csv files (with different N)

Process Output: Best scenario. Best Algorithm. Best N.

