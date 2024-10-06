# About The Forage

The Forage Job Simulations are online, interactive programs designed to give students and job seekers a hands-on experience with real-world tasks from various industries. These simulations allow participants to explore different career roles by completing tasks similar to what they would encounter in actual jobs, providing practical insights into fields like law, finance, technology, and consulting. The purpose of The Forage is to help individuals build job-relevant skills, enhance their resumes, and gain a better understanding of career paths before entering the workforce, all while allowing companies to engage with potential talent.

## Commonwealth Bank Introduction to Cybersecurity

I completed a job simulation focused on the role of a cybersecurity generalist specializing in fraud detection and prevention for Commonwealth Bank's Cybersecurity team. Through this job simulation, I developed skills in building data visualization dashboards using Splunk to uncover patterns and insights in historical customer data. Which aided in the detection of potential fraud. I also demonstrated the ability to respond effectively to cybersecurity incidents. Actions including notifying relevant teams, collecting critical information, containing and stopping attacks, and assisting in recovery efforts. Additionally, I enhanced my security awareness expertise by designing infographics promoting best practices for secure password management, following Australian Cybersecurity Center guidelines. I also gained practical experience in penetration testing, assessing web application security, identifying vulnerabilities, and providing recommendations to strengthen cybersecurity defenses.

<a href="https://github.com/AaronRMartinez/TheForage-Commonwealth-Bank-Job-Simulation/blob/main/Commonwealth%20Bank%20Certificate%20of%20Completion.pdf">Commonwealth Bank Introduction to Cybersecurity Certifcate of Completion</a>

### Task 1: Utilizing Splunk Enterprise for Fraud-Related Data

For this task, I installed and set up Splunk Enterprise to analyze a provided dataset focused on fraud-related data. After successfully importing the dataset, I utilized Splunk's powerful data exploration tools to investigate and identify key patterns. To present the insights, I created a comprehensive dashboard featuring a variety of charts and tables that effectively visualized the fraud data, making it easy to interpret trends and detect suspicious activity. The final dashboard was designed to be clear, informative, and ready for submission, providing a valuable tool for fraud detection and prevention efforts.

[Splunk Dashboard](https://github.com/AaronRMartinez/TheForage-Commonwealth-Bank-Job-Simulation/blob/main/Fraud%20Detection%20Dashboard%20(2024-09-30).pdf)

### Splunk Search Queries

**Transactions by Category:**

```
sourcetype="2fraud_dectection.csv" | top category
```

**Number of Transaction Type:**

```
sourcetype="2fraud_dectection.csv"  | stats count by fraud
```

**Transactions by Age:**

```
sourcetype="2fraud_dectection.csv"  | stats count by age
```

**Fraud Detected by Age:**

```
sourcetype="2fraud_dectection.csv" fraud="1" | stats count by age
```

**Age 19-25 Fraud by Merchant:**

```
sourcetype="2fraud_dectection.csv" fraud="1" age="1" | stats count by merchant
```

**Age 26-35 Fraud by Merchant:**

```
sourcetype="2fraud_dectection.csv" fraud="1" age="2" | stats count by merchant
```

**Fraud Detected by Category:**

```
sourcetype="2fraud_dectection.csv" fraud="1" | stats count values(1) by category
```

**Fraud Detected by Step:**

```
sourcetype="2fraud_dectection.csv" fraud="1" | stats count by step
```

**Fraud Detected by Gender:**

```
sourcetype="2fraud_dectection.csv" fraud="1" | stats count by gender
```

**Transactions by Merchant:**

```
sourcetype="2fraud_dectection.csv"  | stats count by merchant
```

**Fraud Detected by Merchant:**

```
sourcetype="2fraud_dectection.csv" fraud="1" | stats count by merchant
```

**Female Fraud Detected by Category:**

```
sourcetype="2fraud_dectection.csv" fraud="1" gender="F'" | stats count by category
```

**Male Fraud Detected by Category:**

```
sourcetype="2fraud_dectection.csv" fraud="1" gender="M'" | stats count by category
```

### Task 2: Utilizing Splunk Enterprise for Fraud-Related Data

Based on the incident details given, a phishing attack, where employees were tricked into entering their credentials to a credential harvester and to download malware. As a cybersecurity analyst, the next steps call for immediate containment, resolution, and recovery measures. To contain the attack, all affected accounts should be disabled, the malicious website blocked, and malware isolated. For resolution, systems must be scanned and cleaned of any infections, and compromised credentials reset. Recovery actions include restoring file shares from backups, ensuring the systems are fully operational, and monitoring for further signs of compromise. Post-incident, a thorough investigation should be conducted to determine the scope of the breach, followed by security awareness training to prevent future phishing attacks. Implementing stronger email filtering, multi-factor authentication, and monitoring tools will help mitigate similar incidents in the future.

<a href="">Incident Response Replies</a>

