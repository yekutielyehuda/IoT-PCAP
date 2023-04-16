1. https://iotanalytics.unsw.edu.au/iottraces.html

this data was collected for the report given by A. Sivanathan, H. Habibi Gharakheili, F. Loi, A. Radford, C. Wijenayake, A. Vishwanath and V. Sivaraman, "Classifying IoT Devices in Smart Environments Using Network Traffic Characteristics", IEEE Transactions on Mobile Computing, Aug, 2018.
this data can be analyzed by the tool: https://github.com/arunmir/sdn-sim
the list of devices that were used in this research can be found at: https://iotanalytics.unsw.edu.au/resources/List_Of_Devices.txt

2. https://github.com/ArifulIslamPreence/IoT-TCP-Attack-detection

Flow generators Argus and Tranalyzer were used to reduce the raw pcap packets to flows.
PCAP dataset can be downloaded from here --> https://iotanalytics.unsw.edu.au/attack-data

3. https://research.aalto.fi/en/datasets/iot-devices-captures

This dataset represents the traffic emitted during the setup of 31 smart home IoT devices of 27 different types (4 types are represented by 2 devices each). Each setup was repeated at least 20 times per device-type.
Each directory contains several pcap files, each representing a setup of the given device directory. Files are named Setup-X-Y-STA.pcap where X is the person realizing the setup and Y is the sequence number of the given capture. The file _iotdevice-mac.txt contains the MAC address of the considered IoT device.

For analysis of the data look at:
https://research.aalto.fi/en/publications/iot-sentinel-automated-device-type-identification-for-security-en
https://research.aalto.fi/en/publications/iot-sentinel-demo-automated-device-type-identification-for-securi

4. https://www.stratosphereips.org/datasets-iot23

IoT-23 is a new dataset of network traffic from Internet of Things (IoT) devices. It has 20 malware captures executed in IoT devices, and 3 captures for benign IoT devices traffic. It was first published in January 2020, with captures ranging from 2018 to 2019. This IoT network traffic was captured in the Stratosphere Laboratory, AIC group, FEL, CTU University, Czech Republic. Its goal is to offer a large dataset of real and labeled IoT malware infections and IoT benign traffic for researchers to develop machine learning algorithms. This dataset and its research is funded by Avast Software, Prague. 

The IoT-23 dataset consists of twenty three captures (called scenarios) of different IoT network traffic. These scenarios are divided into twenty network captures (pcap files) from infected IoT devices (which will have the name of the malware sample executed on each scenario) and three network captures of real IoT devices network traffic (that have the name of the devices where the traffic was captured). On each malicious scenario we executed a specific malware sample in a Raspberry Pi, that used several protocols and performed different actions. 

![image](https://user-images.githubusercontent.com/83675729/232314001-95bd1bcc-1192-460c-94ff-3020437dee4d.png)
Table: Summary of the Malicious IoT Scenarios

5. https://www.stratosphereips.org/datasets-iot

One of the main goals of Aposemat project is to obtain and use real IoT malware to infect the devices in order to create up to date datasets for research purposes. The datasets will be available to the public and published regularly in the Malware on IoT Dataset page.

We analyze these datasets in a regular basis. Check the blog to make sure you don’t miss our analysis write ups.
the blog is at: https://www.stratosphereips.org/blog


6. https://www.unb.ca/cic/datasets/enricheddataset.html

Enriching IoT datasets
Enriching the existing famous IoT datasets (Bot-IoT and TON-IoT) by employing two general aspects, namely Horizontal and Vertical. Horizontal means proposing new and informative features for datasets. Vertical aspect presents the idea of merging datasets.

Modules
The main directory contains two zip files, namely Datasets and Source_codes.

The Dataset Zip file contains two folders, namely merged_datasets and Original_datasets. 
Source codes
The Source code folder contains our implementation for extracting original and proposed features from PCAP files.
There are seven .py files inside this folder. To execute the source code, you need to navigate to the Generating_dataset.py file. Inside this file, the addresses of PCAP files can be set. The remaining python files present our implementation for different parts. For example, as the names suggest, the Communication_features.py implements the Communication features proposed by us. The Supporting_functions.py demonstrates the supporting functions that are defined to make the extraction process easy. Similarly, we can analyze the remaining files.

To download the dataset:
http://205.174.165.80/IOTDataset/

7. https://ieee-dataport.org/open-access/mqtt-iot-ids2020-mqtt-internet-things-intrusion-detection-dataset

MQTT-IOT-IDS2020: MQTT INTERNET OF THINGS INTRUSION DETECTION DATASET
Message Queuing Telemetry Transport (MQTT) protocol is one of the most used standards used in Internet of Things (IoT) machine to machine communication. The increase in the number of available IoT devices and used protocols reinforce the need for new and robust Intrusion Detection Systems (IDS). However, building IoT IDS requires the availability of datasets to process, train and evaluate these models. The dataset presented in this paper is the first to simulate an MQTT-based network. The dataset is generated using a simulated MQTT network architecture. The network comprises twelve sensors, a broker, a simulated camera, and an attacker. Five scenarios are recorded: (1) normal operation, (2) aggressive scan, (3) UDP scan, (4) Sparta SSH brute-force, and (5) MQTT brute-force attack.  The raw pcap files are saved, then features are extracted. Three abstraction levels of features are extracted from the raw pcap files: (a) packet features, (b) Unidirectional flow features and (c) Bidirectional flow features. The csv feature files in the dataset are suited for Machine Learning (ML) usage. Also, the raw pcap files are suitable for the deeper analysis of MQTT IoT networks communication and the associated attacks. 

Instructions: 
The dataset consists of 5 pcap files, namely, normal.pcap, sparta.pcap, scan_A.pcap, mqtt_bruteforce.pcap and scan_sU.pcap. Each file represents a recording of one scenario; normal operation, Sparta SSH brute-force, aggressive scan, MQTT brute-force and UDP scan respectively. The attack pcap files contain background normal operations. The attacker IP address is “192.168.2.5”. Basic packet features are extracted from the pcap files into CSV files with the same pcap file names. The features include flags, length, MQTT message parameters, etc. Later, unidirectional and bidirectional features are extracted.  It is important to note that for the bidirectional flows, some features (pointed as *) have two values—one for forward flow and one for the backward flow. The two features are recorded and distinguished by a prefix “fwd_” for forward and “bwd_” for backward. 

To download the datasets:
https://ieee-dataport.org/data-formats/pcap-zip
https://ieee-dataport.org/data-formats/csv-zip-0

8. https://mcfp.felk.cvut.cz/publicDatasets/IoT-23-Dataset/

Aposemat IoT-23: A labeled dataset with malicious and benign IoT network traffic.
This IoT network traffic was captured in the Stratosphere Laboratory, AIC group, FEL, CTU University, Czech Republic. Its goal is to offer a large dataset of real and labeled IoT malware infections and IoT benign traffic for researchers to develop machine learning algorithms. This dataset and its research is funded by Avast Software, Prague.

Description
The IoT-23 dataset consists of twenty three captures (called scenarios) of different IoT network traffic. These scenarios are divided into twenty network captures (pcap files) from infected IoT devices and three network captures of real IoT devices network traffic. On each malicious scenario we executed a specific malware in a Raspberry Pi, that used several protocols and performed different actions. The network traffic capture for the bening scenarios was obtained by capturing the network traffic of three different IoT devices: a Philips HUE smart LED lamp, an Amazon Echo home intelligent personal assistant and a Somfy smart doorlock. It is important to mention that these three IoT devices are real hardware and not simulated. This allows us to capture and analyze real network behaviour. Both malicious and benign scenarios run in a controlled network environment with unrestrained internet connection like any other real IoT device.

The following table summarized each scenario and its basic characteristics. See a more comprehensive detail of each scenario at [IoT-23 Dataset] (https://www.stratosphereips.org/datasets-iot23)

Scenario #	Type	Capture Name	Malware/Device	Duration	Number of Packets	Total Flows	Total Size (GB)
Scenario 1	Malicious	CTU-IoT-Malware-Capture-34-1	Mirai	24.000	233,000	23,146.000	0.121
Scenario 2	Malicious	CTU-IoT-Malware-Capture-43-1	Mirai	1.000	82,000,000	67,321,810.000	6.000
Scenario 3	Malicious	CTU-IoT-Malware-Capture-44-1	Mirai	2.000	1,309,000	238.000	1.700
Scenario 4	Malicious	CTU-IoT-Malware-Capture-49-1	Mirai	8.000	18,000,000	5,410,562.000	1.300
Scenario 5	Malicious	CTU-IoT-Malware-Capture-52-1	Mirai	24.000	64,000,000	19,781,379.000	4.600
Scenario 6	Malicious	CTU-IoT-Malware-Capture-20-1	Torii	24.000	50,000	3,210.000	0.004
Scenario 7	Malicious	CTU-IoT-Malware-Capture-21-1	Torii	24.000	50,000	3,287.000	0.004
Scenario 8	Malicious	CTU-IoT-Malware-Capture-42-1	Trojan	8.000	24,000	4,427.000	0.003
Scenario 9	Malicious	CTU-IoT-Malware-Capture-60-1	Gagfyt	24.000	271,000,000	3,581,029.000	21.000
Scenario 10	Malicious	CTU-IoT-Malware-Capture-17-1	Kenjiro	24.000	109,000,000	54,659,864.000	7.800
Scenario 11	Malicious	CTU-IoT-Malware-Capture-36-1	Okiru	24.000	13,000,000	13,645,107.000	0.992
Scenario 12	Malicious	CTU-IoT-Malware-Capture-33-1	Kenjiro	24.000	54,000,000	54,454,592.000	3.900
Scenario 13	Malicious	CTU-IoT-Malware-Capture-8-1	Hakai	24.000	23,000	10,404.000	0.002
Scenario 14	Malicious	CTU-IoT-Malware-Capture-35-1	Mirai	24.000	46,000,000	10,447,796.000	3.600
Scenario 15	Malicious	CTU-IoT-Malware-Capture-48-1	Mirai	24.000	13,000,000	3,394,347.000	1.200
Scenario 16	Malicious	CTU-IoT-Malware-Capture-39-1	IRCBot	7.000	73,000,000	73,568,982.000	5.300
Scenario 17	Malicious	CTU-IoT-Malware-Capture-7-1	Linux,Mirai	24.000	11,000,000	11,454,723.000	0.897
Scenario 18	Malicious	CTU-IoT-Malware-Capture-9-1	Linux.Hajime	24.000	6,437,000	6,378,294.000	0.472
Scenario 19	Malicious	CTU-IoT-Malware-Capture-3-1	Muhstik	36.000	496,000	156,104.000	0.056
Scenario 20	Malicious	CTU-IoT-Malware-Capture-1-1	Hide and Seek	112.000	1,686,000	1,008,749.000	0.140
Scenario 21	Benign	CTU-Honeypot-Capture-7-1	Soomfy Doorlock	1.4	8,276	139.000	0.002
Scenario 22	Benign	CTU-Honeypot-Capture-4-1	Phillips HUE	24.000	21,000.000	461.000	0.004
Scenario 23	Benign	CTU-Honeypot-Capture-5-1	Amazon Echo	5.400	398,000.000	1,383.000	0.364

The password of the zip files for the binaries on each scenario is: infected

10. https://github.com/yliang725/Anomaly-Detection-IoT23

This project is part of the research under
Machine Learning and Deep Learning Methods for Better Anomaly Detection in IoT-23 Dataset Cybersecurity.

The goal of the research was to find the best solution based on time efficiency and accuracy.
This paper proposed an anomaly detection system model for IoT security with the implementation of ML/DL methods, including Naïve Bayes, SVM, Decision Trees, and CNN.
The proposed method reached better accuracy compared to other paper.
The research was performed on the IoT-23 dataset.
Data Preprocessing
This file is the data preprocessing for IoT-23 dataset. It loads 23 datasets seprately into Pandas dataframe, then skip the first 10 rows (headers) and load the 100,000 rows after. When finished, it combines 23 dataframes into a new dataset:
iot23_combined.csv
Note: The lighter version (8.8GB) of IoT-23 dataset was used in this research.

Models
There are total of 4 models are implemented in this project:

CNN
SVM
Decision Trees
Navie Bayes
Environment Settings
Anaconda Jupyter Notebook
Python 3.8
Tensorflow 2.4

12. https://github.com/Iretha/IoT23-network-traffic-anomalies-classification

Detection and Classification of Network Traffic Anomalies
Experiments are based on the light version of IoT-23 dataset.
