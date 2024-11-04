Modbus TCP Exhaustion Packet Generator
Description
The Modbus TCP Exhaustion Packet Generator simulates a Denial-of-Service (DoS) attack against a Modbus TCP server by generating a high volume of requests. This tool can be used for testing server resilience under heavy load conditions.

Features

Simulates Modbus TCP requests with random IP and MAC addresses.
Generates ARP and TCP packets to exhaust server resources.
Logs each request to a CSV file for further analysis.
Requirements

Python packages: scapy, random, subprocess
Network interface setup for sending and receiving packets.
How to Run

Set the target_ip and target_port to the IP and port of the Modbus TCP server.
Run the script to begin packet generation.
Logs are saved in Logging_Data3.csv.
SYN Flood Attack Detection
Description
This project uses a RandomForest classifier to detect SYN flood attacks based on network packet data. The classifier is trained on labeled packet data and predicts potential attacks in test datasets.

Features

Uses RandomForestClassifier from Scikit-Learn for robust classification.
Performs grid search to optimize model parameters.
Outputs prediction results and generates a learning curve.
Requirements

Python packages: scikit-learn, pandas, seaborn, matplotlib
Dataset files (training and testing) in CSV format.
How to Run

Place your training data in Private_measuring/training1a.csv and testing data in Private_measuring/testing1a.csv.
Run the script to train the model and predict SYN flood attacks on the test set.
The output with predictions will be saved as predicted_testing1a_with_original_ips_2.csv.
License
This repository is licensed under the Apache License 2.0. See the LICENSE file for details.

Note: The datasets used in this project are licensed under the Creative Commons Attribution 4.0 License.

Author Information
Developed by Zoltan DOBRADY.
Contact: zoltan.dobrady@hotmail.com ​​
