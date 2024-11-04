# Modbus TCP Exhaustion Packet Generator & SYN Flood Attack Detection

This repository contains two key projects developed for network security purposes:

1. **Modbus TCP Exhaustion Packet Generator**: A tool to simulate Modbus TCP exhaustion attacks.
2. **SYN Flood Attack Detection**: A RandomForest-based classifier for detecting SYN flood attacks.

Both projects are released under the Apache License 2.0.

---

## Contents

- [Modbus TCP Exhaustion Packet Generator](#modbus-tcp-exhaustion-packet-generator)
- [SYN Flood Attack Detection](#syn-flood-attack-detection)
- [License](#license)

---

### Modbus TCP Exhaustion Packet Generator

**Description**  
The Modbus TCP Exhaustion Packet Generator simulates a Denial-of-Service (DoS) attack against a Modbus TCP server by generating a high volume of requests. This tool can be used for testing server resilience under heavy load conditions.

**Features**
- Simulates Modbus TCP requests with random IP and MAC addresses.
- Generates ARP and TCP packets to exhaust server resources.
- Logs each request to a CSV file for further analysis.

**Requirements**
- Python packages: `scapy`, `random`, `subprocess`
- Network interface setup for sending and receiving packets.

**How to Run**
1. Set the `target_ip` and `target_port` to the IP and port of the Modbus TCP server.
2. Run the script to begin packet generation.
3. Logs are saved in `Logging_Data3.csv`.

---

### SYN Flood Attack Detection

**Description**  
This project uses a RandomForest classifier to detect SYN flood attacks based on network packet data. The classifier is trained on labeled packet data and predicts potential attacks in test datasets.

**Features**
- Uses `RandomForestClassifier` from Scikit-Learn for robust classification.
- Performs grid search to optimize model parameters.
- Outputs prediction results and generates a learning curve.

**Requirements**
- Python packages: `scikit-learn`, `pandas`, `seaborn`, `matplotlib`
- Dataset files (training and testing) in CSV format.

**How to Run**
1. Place your training data in `Private_measuring/training1a.csv` and testing data in `Private_measuring/testing1a.csv`.
2. Run the script to train the model and predict SYN flood attacks on the test set.
3. The output with predictions will be saved as `predicted_testing1a_with_original_ips_2.csv`.

---

## License

This repository is licensed under the Apache License 2.0. See the [LICENSE](./LICENSE) file for details.

**Note**: The datasets used in this project are licensed under the Creative Commons Attribution 4.0 License.

---

### Author Information
- Developed by **Zoltan DOBRADY**.
- Contact: [zoltan.dobrady@hotmail.com](mailto:zoltan.dobrady@hotmail.com)
