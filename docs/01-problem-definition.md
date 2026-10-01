# 01 — Problem Definition

## 1. Project Title

**Intelligent Network Traffic Anomaly Detection and Predictive Analysis Using Machine Learning**

Short name: **NetGuard ML**

---

## 2. Background

Modern computer networks continuously generate large volumes of network traffic as devices communicate with servers, applications, and other devices.

Network traffic contains information about communication behaviour such as IP addresses, ports, protocols, packet counts, data volume, flow duration, and other statistical characteristics.

Analysing these characteristics can help identify unusual traffic behaviour.

---

## 3. What is Network Traffic?

Network traffic refers to the data exchanged between devices over a network.

Examples include:

- Web requests
- DNS queries
- Video streaming
- File transfers
- API communication
- Database communication

Each communication generates measurable characteristics that can be used to analyse network behaviour.

---

## 4. Packet and Network Flow

A **packet** is an individual unit of data transmitted through a network.

A **network flow** represents a sequence of packets belonging to the same communication between endpoints.

Flow-level information can include:

- Source IP
- Destination IP
- Source port
- Destination port
- Protocol
- Flow duration
- Number of packets
- Number of bytes
- Packet rate
- Byte rate
- Other statistical characteristics

This project will primarily work with network-flow-level data.

---

## 5. What is a Network Anomaly?

A network anomaly is a traffic behaviour that significantly differs from an expected or learned pattern.

Examples may include:

- Sudden traffic spikes
- Unusually high packet rates
- Abnormal connection patterns
- Unexpected protocol behaviour
- Repeated connection attempts
- Unusual data transfer volumes

An anomaly does not automatically mean that the traffic is malicious.

A legitimate event such as a large file transfer or software update can also produce unusual traffic.

Therefore, the initial objective of this project is to detect **anomalous behaviour**, rather than automatically classifying every anomaly as an attack.

---

## 6. Problem Statement

Modern networks generate large volumes of traffic, making manual identification of unusual behaviour difficult.

Changes in traffic volume, packet characteristics, connection patterns, or protocol behaviour may indicate congestion, misconfiguration, scanning, flooding, or other abnormal behaviour.

The goal of this project is to develop a machine-learning-based system that learns network traffic patterns, detects anomalous behaviour, analyses the characteristics contributing to the anomaly, and explores prediction of future traffic trends.

---

## 7. Why Machine Learning?

Traditional rule-based systems often rely on manually defined thresholds.

For example:

```text
IF packet_rate > threshold
THEN mark traffic as suspicious

---

## 8. Project Objective

The project aims to develop a pipeline that can:

1. Understand network traffic behaviour.
2. Preprocess network-flow data.
3. Analyse important traffic features.
4. Detect anomalous traffic behaviour.
5. Quantify the degree of abnormality using anomaly scores where appropriate.
6. Analyse the characteristics associated with detected anomalies.
7. Explore prediction of future traffic trends.
8. Visualize traffic patterns and detected anomalies.

---

## 9. Project Pipeline

Network Traffic Data
        ↓
Data Preprocessing
        ↓
Feature Analysis
        ↓
Anomaly Detection
        ↓
Anomaly Scoring
        ↓
Anomaly Explanation
        ↓
Traffic Trend Prediction
        ↓
Visualization