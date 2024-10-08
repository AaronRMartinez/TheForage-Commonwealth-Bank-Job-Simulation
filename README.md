# About The Forage

The Forage Job Simulations are online, interactive programs designed to give students and job seekers a hands-on experience with real-world tasks from various industries. These simulations allow participants to explore different career roles by completing tasks similar to what they would encounter in actual jobs, providing practical insights into fields like law, finance, technology, and consulting. The purpose of The Forage is to help individuals build job-relevant skills, enhance their resumes, and gain a better understanding of career paths before entering the workforce, all while allowing companies to engage with potential talent.

## Commonwealth Bank Introduction to Cybersecurity

I completed a job simulation focused on the role of a cybersecurity generalist specializing in fraud detection and prevention for Commonwealth Bank's Cybersecurity team. Through this job simulation, I developed skills in building data visualization dashboards using Splunk to uncover patterns and insights in historical customer data. Which aided in the detection of potential fraud. I also demonstrated the ability to respond effectively to cybersecurity incidents. Actions including notifying relevant teams, collecting critical information, containing and stopping attacks, and assisting in recovery efforts. Additionally, I enhanced my security awareness expertise by designing infographics promoting best practices for secure password management, following Australian Cybersecurity Center guidelines. I also gained practical experience in penetration testing, assessing web application security, identifying vulnerabilities, and providing recommendations to strengthen cybersecurity defenses.

<a href="https://github.com/AaronRMartinez/TheForage-Commonwealth-Bank-Job-Simulation/blob/main/Commonwealth%20Bank%20Certificate%20of%20Completion.pdf">Commonwealth Bank Introduction to Cybersecurity Certifcate of Completion</a>

### Task 1: Utilizing Splunk Enterprise for Fraud-Related Data

For this task, I installed and set up Splunk Enterprise to analyze a provided dataset focused on fraud-related data. After successfully importing the dataset, I utilized Splunk's powerful data exploration tools to investigate and identify key patterns. To present the insights, I created a comprehensive dashboard featuring a variety of charts and tables that effectively visualized the fraud data, making it easy to interpret trends and detect suspicious activity. The final dashboard was designed to be clear, informative, and a valuable tool for fraud detection and prevention efforts.

[Splunk Dashboard](https://github.com/AaronRMartinez/TheForage-Commonwealth-Bank-Job-Simulation/blob/main/Fraud%20Detection%20Dashboard%20(2024-09-30).pdf)

![Splunk Dashboard](https://github.com/AaronRMartinez/TheForage-Commonwealth-Bank-Job-Simulation/blob/main/Commonwealth%20Bank%20Splunk%20Dashboard%20Screenshot.jpg)

![Splunk Dashboard 2](https://github.com/AaronRMartinez/TheForage-Commonwealth-Bank-Job-Simulation/blob/main/Commonwealth%20Bank%20Splunk%20Dashboard%20Screenshot%202.jpg)

### Splunk Search Queries

**Transactions by Category:**

```
sourcetype="fraud_dectection.csv" | top category
```

**Number of Transaction Type:**

```
sourcetype="fraud_dectection.csv"  | stats count by fraud
```

**Transactions by Age:**

```
sourcetype="fraud_dectection.csv"  | stats count by age
```

**Fraud Detected by Age:**

```
sourcetype="fraud_dectection.csv" fraud="1" | stats count by age
```

**Age 19-25 Fraud by Merchant:**

```
sourcetype="fraud_dectection.csv" fraud="1" age="1" | stats count by merchant
```

**Age 26-35 Fraud by Merchant:**

```
sourcetype="fraud_dectection.csv" fraud="1" age="2" | stats count by merchant
```

**Fraud Detected by Category:**

```
sourcetype="fraud_dectection.csv" fraud="1" | stats count values(1) by category
```

**Fraud Detected by Step:**

```
sourcetype="fraud_dectection.csv" fraud="1" | stats count by step
```

**Fraud Detected by Gender:**

```
sourcetype="fraud_dectection.csv" fraud="1" | stats count by gender
```

**Transactions by Merchant:**

```
sourcetype="fraud_dectection.csv"  | stats count by merchant
```

**Fraud Detected by Merchant:**

```
sourcetype="fraud_dectection.csv" fraud="1" | stats count by merchant
```

**Female Fraud Detected by Category:**

```
sourcetype="fraud_dectection.csv" fraud="1" gender="F'" | stats count by category
```

**Male Fraud Detected by Category:**

```
sourcetype="fraud_dectection.csv" fraud="1" gender="M'" | stats count by category
```

### Task 2: Analysis of an Incident

For this task, I was responsible for identifying the type of cyber attack based on the incident details, analyzing indicators such as the attack method and compromised assets. Once the attack was identified, I was required to outline the necessary steps for containment, resolution, and recovery, ensuring that the threat were isolated, the damage mitigated, and the systems restored. I developed a detailed list of actions to contain the attack, such as isolating affected systems and resetting credentials, followed by resolving any vulnerabilities and cleaning infected systems. After the recovery, I conducted post-incident activities like reviewing the attack's root cause, implementing stronger security controls, and recommending employee training or security awareness programs to prevent future incidents.

<a href="https://github.com/AaronRMartinez/TheForage-Commonwealth-Bank-Job-Simulation/blob/main/Commonwealth%20Incident%20Report.pdf">Incident Response Replies</a>

### Task 3: Enhancing Password Security Awareness: Infographic Development

The task involved researching the Australian Cyber Security Centre's (ACSC) guidelines for secure passwords. Then designing a visually appealing and clear infographic using design software such as Canva. With the completed infographic, it was formatted into an easy-to-understand PDF for distribution to fellow employees, with a focus on enhancing password security awareness.

<a href="https://github.com/AaronRMartinez/TheForage-Commonwealth-Bank-Job-Simulation/blob/main/ACSC%20Password%20Practices.pdf">ACSC Secure Password Practices Infographic</a>

### Task 4: Penetration Testing Skill Development through HackThisSite Challenges

This task involved creating an account on HackThisSite and completing all 11 levels of the "Basic" web challenges. Following this, a Penetration Testing Report was documented, which included an executive summary, scope, descriptions of vulnerabilities, key findings, and security recommendations for each challenge level. The knowledge gained from these challenges could be applied to real-world scenarios to enhance penetration testing skills.

<a href="https://github.com/AaronRMartinez/TheForage-Commonwealth-Bank-Job-Simulation/blob/main/Commonwealth%20Bank%20Penetration%20Testing%20Report.pdf">Penetration Testing Report on HackThisSite Basic Challenges</a>
