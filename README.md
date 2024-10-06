# About The Forage

The Forage Job Simulations are online, interactive programs designed to give students and job seekers a hands-on experience with real-world tasks from various industries. These simulations allow participants to explore different career roles by completing tasks similar to what they would encounter in actual jobs, providing practical insights into fields like law, finance, technology, and consulting. The purpose of The Forage is to help individuals build job-relevant skills, enhance their resumes, and gain a better understanding of career paths before entering the workforce, all while allowing companies to engage with potential talent.

## Commonwealth Bank Introduction to Cybersecurity

I completed a job simulation focused on the role of a cybersecurity generalist specializing in fraud detection and prevention for Commonwealth Bank's Cybersecurity team. Through this job simulation, I developed skills in building data visualization dashboards using Splunk to uncover patterns and insights in historical customer data. Which aided in the detection of potential fraud. I also demonstrated the ability to respond effectively to cybersecurity incidents. Actions including notifying relevant teams, collecting critical information, containing and stopping attacks, and assisting in recovery efforts. Additionally, I enhanced my security awareness expertise by designing infographics promoting best practices for secure password management, following Australian Cybersecurity Center guidelines. I also gained practical experience in penetration testing, assessing web application security, identifying vulnerabilities, and providing recommendations to strengthen cybersecurity defenses.

<a href="https://github.com/AaronRMartinez/TheForage-Commonwealth-Bank-Job-Simulation/blob/main/Commonwealth%20Bank%20Certificate%20of%20Completion.pdf">Commonwealth Bank Introduction to Cybersecurity Certifcate of Completion</a>

### Task 1: Utilizing Splunk Enterprise for Fraud-Related Data

For this task, I installed and set up Splunk Enterprise to analyze a provided dataset focused on fraud-related data. After successfully importing the dataset, I utilized Splunk's powerful data exploration tools to investigate and identify key patterns. To present the insights, I created a comprehensive dashboard featuring a variety of charts and tables that effectively visualized the fraud data, making it easy to interpret trends and detect suspicious activity. The final dashboard was designed to be clear, informative, and ready for submission, providing a valuable tool for fraud detection and prevention efforts.

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
