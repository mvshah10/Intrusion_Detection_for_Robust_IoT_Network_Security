# Intrusion Detection for Robust IoT Network Security
 
## Description

In today's rapidly evolving digital landscape, the proliferation of Internet of Things (IoT) devices has brought unparalleled convenience and connectivity. However, this interconnectedness also introduces significant security challenges. The alarming rise in cyber threats, ranging from unauthorized access to data breaches and denial of service attacks, has underscored the critical need for robust intrusion detection and prevention mechanisms in IoT network security.

As the IoT ecosystem continues to expand, ensuring the integrity, confidentiality, and availability of sensitive data becomes paramount. An effective intrusion detection system serves as a vigilant guardian against unauthorized activities and malicious actors, enabling proactive threat identification and swift response. By deploying sophisticated detection models and leveraging advanced machine learning techniques, we can fortify IoT network security and safeguard the privacy and functionality of connected devices.

## Features

- Real-time intrusion detection algorithms
- Machine learning models for anomaly detection
- Data preprocessing and feature engineering techniques
- Interactive visualization of network traffic patterns
- Continuous monitoring and alerting mechanisms

## Datasets

https://research.unsw.edu.au/projects/unsw-nb15-dataset

## Data:
This data set has a hybrid of the real modern normal and the contemporary synthesized attack activities of the network traffic. Existing and novel methods are utilised to generate the features of the UNSW- NB15 data set.

 Field Name  | Description |
 ----------- | ----------- |
| id          | unique identifier for each attack |
| dur         | Record total duration         |
| proto       | Transaction protocol      |
| service     | http, ftp, ssh, dns ..,else (-) |
| state       | The state and its dependent protocol, e.g. ACC, CLO, else (-) |
| spkts       | Source to destination packet count |
| dpkts       | Destination to source packet count |
| sbytes      | Source to destination bytes         |
| dbytes      | Destination to source bytes|
| rate        | The avrage attack rate           |
| sttl        | Source to destination time to live         |
| dttl        | Destination to destination time to live     | 
| sload       | Source packets retransmitted or dropped      |
| dload       | Destination packets retransmitted or dropped      |
| sloss       | Source packets retransmitted or dropped
| dloss       | Destination packets retransmitted or dropped     |
| sinpkt      | Source inter-packet arrival time (mSec)         |
| dinpkt      | Destination inter-packet arrival time (mSec)    |
| sjit        | Source jitter (mSec)                            |
| djit        | Destination jitter (mSec)                     |
| swin        | Source TCP window advertisement               |
| dwin        | Destination TCP window advertisement          |
| stcpb       | Source TCP sequence number                    |
| dtcpb       | Destination TCP sequence number               |
| tcprtt      | The sum of ’synack’ and ’ackdat’ of the TCP   |
| synack      | The time between the SYN and the SYN_ACK packets of the TCP |
| ackdat      | The time between the SYN_ACK and the ACK packets of the TCP |
| smean       | Mean of the flow packet size transmitted by the src         |
| dmean       | Mean of the flow packet size transmitted by the dst         |
| trans_depth | the depth into the connection of http request/response transaction |
| response_body_len | The content size of the data transferred from the server’s http service |
| ct_srv_src         | No. of connections that contain the same service and destination address in 100 connections according to the last time |
| ct_state_ttl       | No. for each state according to specific range of values for source/destination time to live       |
| ct_dst_ltm         | No. of connections of the same destination address in 100 connections according to the last time        | 
| ct_src_dport_ltm   | No of connections of the same source address  and the destination port  in 100 connections according to the last time    | 
| ct_dst_sport_ltm   | No of connections of the same destination address and the source port in 100 connections according to the last time    |
| ct_dst_src_ltm     | No of connections of the same source and the destination address in in 100 connections according to the last time   | 
| is_ftp_login       | If the ftp session is accessed by user and password then 1 else 0     | 
| ct_ftp_cmd         | No of flows that has a command in ftp session |
| ct_flw_http_mthd   | No. of flows that has methods such as Get and Post in http service        | 
| ct_src_ltm         | No. of connections of the same destination address in 100 connections according to the last time     |
| ct_srv_dst         | No. of connections that contain the same service and destination address in 100 connections according to the last time        |
| is_sm_ips_ports    |  If source equals to destination IP addresses and port numbers are equal, this variable takes value 1 else 0        |
| attack_cat | The name of each attack category. In this data set, nine categories (e.g., Fuzzers, Analysis, Backdoors, DoS, Exploits, Generic, Reconnaissance, Shellcode and Worms) |
| label | 0 for normal and 1 for attack records |

## Machine Learning Models
- Linear Regression Model
- Logistic Regression Model
- Linear Support Vector Machine
- K-Nearest-Neighbor Classifier
- Random Forest Classifier
- Decision Tree Classifier
- Multi Layer Perceptron Classifier
- XGBoost Classifier
- LSTM
- Bidirectional LSTM
- GRU
- Feedforward Neural Network

## Citations

1. Moustafa, Nour, and Jill Slay. "UNSW-NB15: a comprehensive data set for network intrusion detection systems (UNSW-NB15 network data set)." Military Communications and Information Systems Conference (MilCIS), 2015. IEEE, 2015.
2. Moustafa, Nour, and Jill Slay. "The evaluation of Network Anomaly Detection Systems: Statistical analysis of the UNSW-NB15 dataset and the comparison with the KDD99 dataset." Information Security Journal: A Global Perspective (2016): 1-14.
3. Moustafa, Nour, et al. "Novel geometric area analysis technique for anomaly detection using trapezoidal area estimation on large-scale networks." IEEE Transactions on Big Data (2017).
4. Moustafa, Nour, et al. "Big data analytics for intrusion detection system: statistical decision-making using finite dirichlet mixture models." Data Analytics and Decision Support for Cybersecurity. Springer, Cham, 2017. 127-156.
5. Sarhan, Mohanad, Siamak Layeghy, Nour Moustafa, and Marius Portmann. NetFlow Datasets for Machine Learning-Based Network Intrusion Detection Systems. In Big Data Technologies and Applications: 10th EAI International Conference, BDTA 2020, and 13th EAI International Conference on Wireless Internet, WiCON 2020, Virtual Event, December 11, 2020, Proceedings (p. 117). Springer Nature.
