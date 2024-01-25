#It is recommended to begin by reading the directories in the order provided here.
##First Subdirectory: Data-Preprocessing
This subdirectory contains codes implemented for executing the initial processing operation. The purpose of this process is to extract features at the packet level and add attack names corresponding to each packet group. Subsequently, the data is cleaned to prepare it for entry into the classifier model.

Process Input: IoT-23 Dataset (Flow-based dataset)
Process Output: Npacket.csv file (Packet-based dataset)

##Second Subdirectory: Experiments
This subdirectory contains the classifier model applied to the derived dataset, following experiments that include the following:

Application of four algorithms:
1- Random forest.
2- XGBoost.
3- LSTM.
4- KNN.

All these algorithms are implemented for the following cases:
N=1
N=2
.
.
.
N=5
N=10
N=15
N=20
N: Number of packets from each flow.

The execution was also conducted based on two scenarios:

Scenario 1: With port numbers.
Scenario 2: Without port numbers.
Process Input: Npacket.csv files (with different N)
Process Output: Best scenario.
Best Algorithm.
Best N.
