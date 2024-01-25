## This folder contains five separate subdirectories.

<img src="https://github.com/MakaremHind/Detection-of-Botnet-Attacks-Targeting-IoT-Devices/assets/144903433/0b6680f6-0761-4ba9-8be4-47c804ff9b28" width="550" height="550"/>

## First Subdirectory: Editcap Commands
This subdirectory contains instructions for splitting large files into smaller ones based on the number of packets in each file.
- Input File Type: PCAP files
- Output File Type: PCAP files

## Second Subdirectory: Tshark Commands
This subdirectory contains instructions for extracting packet-level features and storing them in files of a different type.
- Input File Type containing features: PCAP files
- Output File Type after applying instructions: CSV files

## Third Subdirectory: Python Code 0
This subdirectory contains Python code that reads files containing flow-level features and stores them in another type of file for easier handling.
- Input File Type: Log.Labeled
- Output File Type: Log.csv

## Fourth Subdirectory: Python Code 1
This subdirectory contains Python code that matches each flow with the set of packets it belongs to. After the matching process, the type of anomaly in the flow is added to the output file.
- Input File Types: Log.csv & CSV files
- Output File Type: AllPacket File with Labels

## Fifth Subdirectory: Python Code 2
This subdirectory contains Python code that cleans the input file data and reshapes the lines to obtain readings for packets within windows. Each line in the output file contains a window with the corresponding anomaly type.
- Input File Type: Allpacket.csv
- Output File Type: Npacket.csv
