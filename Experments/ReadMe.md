
This folder contains three separate subdirectories.
## First Subdirectory: 
Splitting Nmax into Multiple N Files

This subdirectory contains the source code that was used to gradually reduce the packet window as follows:

![Screenshot 2024-01-25 085047](https://github.com/MakaremHind/Detection-of-Botnet-Attacks-Targeting-IoT-Devices/assets/144903433/245fd887-07b6-48e8-a11c-e1b3dd33c1c6)

- Take a window containing 20 packets from the beginning of each flow.
- Take a window containing 15 packets from the beginning of each flow.
- Take a window containing 10 packets from the beginning of each flow.
- Take a window containing 5 packets from the beginning of each flow.
- Take a window containing 4 packets from the beginning of each flow.
.
.
.
- Take a window containing one packet from the beginning of each flow.
  
Finally, all results were stored in separate files.

## Second Subdirectory:
### Scenario Number 1
This is the scenario where port numbers were adopted as features in the training and testing dataset. In this scenario, the following algorithm was applied:

1- Random Forest.
2- XGBoost.
3- LSTM.
4- KNN.
The algorithm application process was performed on all packet numbers taken from the beginning of each flow mentioned above. Therefore, there are 8 codes inside this subdirectory, with each code dedicated to a specific number of packets.

## Third Subdirectory: 
### Scenario Number 2
This is the scenario where port numbers were deleted from the features in the training and testing dataset. In this scenario, the same algorithms were applied as in Scenario Number 1, and the algorithm application process was performed on all packet numbers taken from the beginning of each flow mentioned above. Therefore, there are 8 codes inside this subdirectory, with each code dedicated to a specific number of packets.
