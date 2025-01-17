<h1 style="color:#4CAF50; text-align:center; font-size:3em;">CI/CD DevSecOps Lab</h1>
<hr style="border: 1px solid #ddd;" />

<h2 style="color:#2196F3;">Description</h2>
<p style="font-size:1.2em; line-height:1.6;">
This project demonstrates my implementation of a CI/CD pipeline integrated with security tools to ensure secure software development practices. I worked on a fork of the <a href="https://github.com/nanuchi/devsecops-crash-course-pygoat" style="color:#FF5722; text-decoration:none;">DevSecOps Crash Course PyGoat</a> repository, focusing on incorporating Static Application Security Testing (SAST) and container image scanning into the development lifecycle.
</p>

<hr style="border: 1px solid #ddd;" />

<h2 style="color:#2196F3;">Languages and Utilities Used</h2>
<ul style="font-size:1.2em; list-style-type:square; padding-left:20px;">
  <li><b>Python</b></li>
  <li><b>Docker</b></li>
  <li><b>Bandit</b> (Static Application Security Testing Tool)</li>
</ul>

<h2 style="color:#2196F3;">Environments Used</h2>
<ul style="font-size:1.2em; list-style-type:square; padding-left:20px;">
  <li><b>Ubuntu (GitHub Actions)</b></li>
  <li><b>Docker Hub</b></li>
</ul>

<hr style="border: 1px solid #ddd;" />

<h2 style="color:#2196F3;">Key Components</h2>
<ul style="font-size:1.2em; line-height:1.6; padding-left:20px;">
  <li><b>Static Application Security Testing (SAST):</b> Implemented a CI job to analyze Python code using Bandit, identifying potential security vulnerabilities in the application.</li>
  <li><b>Container Image Scanning:</b> Built a Docker image and scanned it for vulnerabilities using Docker Scout to ensure secure container deployment.</li>
  <li><b>CI/CD Automation:</b> Configured GitHub Actions to automate the security scans, ensuring they run on every push to the repository.</li>
  <li><b>Artifact Management:</b> Collected and stored Bandit scan results for further review and auditing.</li>
</ul>

<hr style="border: 1px solid #ddd;" />

<h2 style="color:#2196F3;">Key Learnings</h2>
<ul style="font-size:1.2em; line-height:1.6; padding-left:20px;">
  <li><b>Static Code Analysis:</b> Gained hands-on experience with Bandit for detecting security vulnerabilities in Python applications.</li>
  <li><b>Container Security:</b> Learned how to use Docker Scout to analyze and address vulnerabilities in container images.</li>
  <li><b>CI/CD Best Practices:</b> Understood the importance of automating security checks to catch vulnerabilities early in the development process.</li>
  <li><b>Tool Integration:</b> Successfully integrated security tools into a CI/CD pipeline using GitHub Actions.</li>
</ul>

<hr style="border: 1px solid #ddd;" />

<h2 style="color:#2196F3;">Challenges Overcome</h2>
<ul style="font-size:1.2em; line-height:1.6; padding-left:20px;">
  <li><b>Setting up Bandit:</b> Ensured proper configuration of Bandit to produce actionable security reports.</li>
  <li><b>Docker Scout Setup:</b> Troubleshot issues related to Docker Scout installation and scanning processes.</li>
  <li><b>Managing Secrets in CI:</b> Configured GitHub repository secrets for secure Docker Hub authentication.</li>
  <li><b>Pipeline Debugging:</b> Resolved errors related to GitHub Actions syntax and step execution during pipeline creation.</li>
</ul>


<h2>Walk-Through:</h2>


<p align="center">
Initial Code to Trigger the Pipeline on any Push: <br/>
<img src="https://i.imgur.com/KvmFF1a.png" height="80%" width="80%" alt="Creating Domain COntroller"/>
<br />
<p align="center">
Configuring SAST Scan: <br/>
<img src="https://i.imgur.com/NC2jJXU.png" height="80%" width="80%" alt="Creating Domain COntroller"/>
<br />
<p align="center">
Bandit Scann Results: <br/>
<img src="https://i.imgur.com/0fPiMEF.png" height="80%" width="80%" alt="Creating Domain COntroller"/>
<br /><p align="center">
Now Configuring Bandit Scan to ignore low severity issues: <br/>
<img src="https://i.imgur.com/46wc7J2.png" height="80%" width="80%" alt="Creating Domain COntroller"/>
<br /><p align="center">
Generate Scan Report and Export as a JSON file: <br/>
<img src="https://i.imgur.com/3TjKvhM.png" height="80%" width="80%" alt="Creating Domain COntroller"/>
<br /><p align="center">
Bandit Scan Report JSON file: <br/>
<img src="https://i.imgur.com/OftAKwu.png" height="80%" width="80%" alt="Creating Domain COntroller"/>
<br /><p align="center">
Configuring Image Scanning with Docker Scout: <br/>
<img src="https://i.imgur.com/UZBSePc.png" height="80%" width="80%" alt="Creating Domain COntroller"/>
<br /><p align="center">
<be />Creating 2 Secert repos to store my Docker Uname and Passwer so I can reference them in the pipeline: <br/>
<img src="https://i.imgur.com/uY94zpc.png" height="80%" width="80%" alt="Creating Domain COntroller"/>
<br />Docker Login Command Reffercing the Secert Values: <br/>
<img src="https://i.imgur.com/KvmFF1a.png" height="80%" width="80%" alt="Creating Domain COntroller"/>
<br />
