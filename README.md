
<h2>Login Security Threat Analysis and Visualization Dashboard</h2

<h1>Login Analysis Dashboard Project Overview</h1>

<p>Conducted a comprehensive analysis and visualization of login data utilizing Splunk, to identify trends, patterns, and anomalies indicative of potential security threats, including brute-force attacks.</p>
<h1>Tool(s)</h1>
  <ul>Splunk</ul>
  
<h1>Project Methodology</h1>

<ul>
<li>Data Ingestion and Indexing: Ingested and indexed login data from Linux Secure logs using Splunk.
  
  <br>
  
<img src="https://i.imgur.com/DKdPkPW.jpeg" height="70%" width="70%" alt="Data Sourcetype"/>
</li>
<p>
  <li>Dashboard Creation for Total Login Attempts: Designed and developed a comprehensive dashboard to display total login attempts.

  <img src="https://i.imgur.com/21HOO4e.png" height="70%" width="70%" alt="Total Login Attempts"></p>
 <img src="https://i.imgur.com/1NgyTRg.png" height="70%" width="70%" alt="Total Login Attempts"></p> 
<img src="https://i.imgur.com/ajzoVhu.png" height="70%" width="70%" alt="Total Login Attempts"></p>
<img src="https://i.imgur.com/M2eJ7Jg.jpeg" height="70%" width="70%" alt="Total Login Attempts"></p>
<img src="https://i.imgur.com/DdP6eKh.png" height="70%" width="70%" alt="Total Login Attempts">
<img src="https://i.imgur.com/qcbToVM.jpeg" height="70%" width="70%" alt="Total Login Attempts">
</li>
<li>Dashboard Creation for Successful Login Attempts: Created a dashboard to display successful login attempts.


<img src="https://i.imgur.com/W7d9LBS.jpeg" height="70%" width="70%" alt="Successful Login Attempts">
<img src="https://i.imgur.com/PkEKsno.jpeg" height="70%" width="70%" alt="Successful Login Attempts">
<img src="https://i.imgur.com/sybVqr7.png" height="70%" width="70%" alt="Successful Login Attempts">

</li>

<li>Dashboard Creation for Failed Login Attempts:Created a dashboard to display failed login attempts by users.


<img src="https://i.imgur.com/AlV1Js2.jpeg" height="70%" width="70%" alt="Failed Login Attempts">
<img src="https://i.imgur.com/d5yuwHF.jpeg" height="70%" width="70%" alt="Failed Login Attempts">
<img src="https://i.imgur.com/x1tq1G5.jpeg" height="70%" width="70%" alt="Failed Login Attempts">

</li>
<li>Dashboard Creation for Failed and Invalid User Login Attempts:Created a dashboard to provide a visual representation of failed password and invalid user.

<img src="https://i.imgur.com/C0rgmlT.jpeg" alt="Failed and invalid Login Attempts">
<img src="https://i.imgur.com/cNWxNPd.jpeg" alt="Failed and invalid Login Attempts">
<img src="https://i.imgur.com/JsnajLO.jpeg" alt="Failed and invalid Login Attempts">
<img src="https://i.imgur.com/ujQh0k2.jpeg" alt="Failed and invalid Login Attempts">
</li>
<li>Dashboard Overview

<img src="https://i.imgur.com/84poV6O.jpeg" alt="Dashboard Overview">
</li>
</ul>

<h1>Login Analysis</h1>

<p>Total Login Attempts: 26,435</p>
<p>Successful: 1,477 (5.59%)</p>
<p>Failed: 24,958 (94.41%)</p>
<p>Failed Login Attempts by Invalid Users: 18,139 (72.68%)</p>
<p>Failed Password Attempts: 6,819 (27.32%)</p>

<h2>Top 10 Countries with Failed Login Attempts:</h2>
<ul>
<li>United Kingdom: 137 failed attempts</li>
<li>China: 128 failed attempts</li>
<li>United States: 126 failed attempts</li>
<li>United States: 115 failed attempts</li>
<li>United Kingdom: 112 failed attempts</li>
<li>Finland: 111 failed attempts</li>
<li>Thailand: 100 failed attempts</li>
<li>Turkey: 98 failed attempts</li>
<li>United States: 95 failed attempts</li>
<li>South Korea: 95 failed attempts</li>
</ul>

<h1>Key Findings</h1>

<ul>
<li>Identified a significant disparity between failure and success rates.</li>
<li>Detected a high count of failed login attempts from multiple countries.</li>
<li>Uncovered potential anomalies and areas for further investigation.</li>
<li>Non-compliance: Regulatory requirements (e.g., PCI-DSS, HIPAA) mandate timestamped logging.
    Audit trail integrity: Timestamps ensure audit trail accuracy and reliability.
</li>
</ul>
<h1>Timestamp is included to give clearer insight</h1>
<li>

<img src="https://i.imgur.com/5j8FVGw.png" alt="With Timestamp">
<img src="https://i.imgur.com/0wMVumi.png" alt="With Timestamp">
<img src="https://i.imgur.com/BUYsCUI.png" alt="With Timestamp">
</li>

<h1>Implications and Recommendations</h1>

<p>The high number of failed login attempts from multiple countries suggests potential malicious activity.This is not 
  limited to failed login attempt even high sucessful login attempts with high can indicate successful brute force attack.
  From the timestamped image above,it can be seen that the user "djohnson" had the highest attempt of 45 on Saturday April
  2nd 2021 at 00:15:02.Its important to note that we may not need to conclude that the user is non malicious or malicious.
  Asides Ip checking,an alternative is to check to check the login intervals within Saturday April 2nd 2021 with probably
  a 5 minutes interval.From here logical deductions can be made as to whether it was maybe a Bruteforce attack or password
  guessing.Nevertheless,the high attempt is really suspicious.Below are some recommendations.
   
</p>

<h1>Recommendations for Incident Response and Threat Mitigation</h1>

<ul>
<li>Enrich Data for Investigation: Utilize databases like AbuseIPDB API for IP address and country information.</li>
<li>Enable Multi-Factor Authentication (MFA): Require MFA for all login attempts.</li>
<li>Implement Rate Limiting: Limit login attempts from single IP addresses.</li>
<li>Conduct Regular Security Audits: Identify and address vulnerabilities.</li>
<li>Monitor Login Activity: Continuously detect and respond to security threats.</li>
<li>Implement Account Lockout Policy: Lock out accounts after failed login attempts.</li>
<li>Direct Outreach and Verification: Verify user identity via voice call.</li>
<li>Remediation: Address malicious activity through IP blocking, account disabling, and investigation.</li>
</ul>

<h1>Conclusion</h1>

<p>This project demonstrated Splunk's effectiveness in login security threat analysis and visualization. The comprehensive dashboard provided valuable insights, enabling identification of potential security threats and anomalies. Findings and recommendations inform incident response and threat mitigation strategies, enhancing security posture and reducing malicious login activity risk.</p>
