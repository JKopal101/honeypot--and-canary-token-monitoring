# Honeypot (Cowrie) and Canary Token Monitoring using a Username MS File

## Project Overview
This project focuses on deploying a honeypot using Cowrie to capture malicious activity and monitoring a Canary Token embedded in a Microsoft Word file containing fake credentials. The aim is to study attacker behaviors and evaluate the effectiveness of deception techniques in cybersecurity.

## Approach & Tools

### Honeypot Deployment:
- Installed and configured Cowrie on a virtual machine to simulate an SSH server.
- Configured logging to capture attacker interactions.

### Canary Token Setup:
- Created a Canary Token embedded in a Microsoft Word document with fake credentials.
- Shared the file in a monitored environment to observe access attempts.

### Monitoring and Analysis:
- Set up email alerts for Canary Token triggers.
- Analyzed captured logs from Cowrie for attacker behaviors.

### Tools Used:
- **Cowrie Honeypot**: For simulating SSH interactions and logging attacker activities.
- **Canary Tokens**: For tracking unauthorized access to the MS Word file.
- **Virtual Machine**: Hosted the honeypot in an isolated environment.

### Suggested Screenshots:
- **Cowrie Configuration**: Screenshot of the configuration file showing key settings.
- **Honeypot Activity Logs**: Screenshot of captured logs showing interaction details.
- **Canary Token Setup**: Screenshot of the Canary Token creation process.

## Implementation & Findings

### Steps Taken:
1. Deployed Cowrie honeypot on an isolated virtual machine and verified its functionality.
2. Configured the honeypot to log commands, file uploads, and interactions.
3. Created a Canary Token linked to a monitored email address.
4. Embedded the token in a Microsoft Word document with fake credentials.
5. Shared the document and monitored the environment for token triggers.
6. Analyzed the collected data for patterns, anomalies, and malicious activities.

### Suggested Screenshots:
- **Honeypot Deployment**: Screenshot of the running Cowrie service.
- **Log Analysis**: Screenshot of analyzed logs showing attacker IPs or commands.
- **Canary Token Alert**: Screenshot of the email alert received upon token activation.

### Key Observations:
- Cowrie captured several SSH login attempts, including brute force attempts.
- Canary Token triggered alerts from unauthorized access to the MS Word file.
- Analysis revealed common attack patterns and tactics used by threat actors.

### Challenges Encountered:
- Maintaining the honeypot in an isolated yet accessible environment.
- Ensuring accurate logging without overwhelming storage resources.
- Fine-tuning the Canary Token to avoid false positives.

## Solutions & Recommendations

### Addressing the Issues:

#### Honeypot Isolation:
- Used firewall rules to limit access while keeping the honeypot visible to attackers.
- Deployed in a sandboxed virtual environment.

#### Log Management:
- Implemented log rotation and archival to manage storage.
- Filtered logs to prioritize high-risk activities.

#### Canary Token Optimization:
- Used unique identifiers to reduce false positives.
- Tested token triggers to ensure reliable alerts.

### Proposed Improvements:
- Deploy additional honeypots mimicking different services (e.g., HTTP, FTP).
- Use advanced log analysis tools to detect complex patterns.
- Integrate Canary Tokens with automation workflows for quicker response.

### Next Steps:
- Expand the scope by deploying honeypots across multiple network segments.
- Regularly update the honeypot configuration to reflect current attack vectors.
- Experiment with different token types (e.g., email or DNS-based tokens).

### Suggested Screenshots:
- **Multi-Service Honeypots**: Screenshot of multiple honeypots running concurrently.
- **Advanced Analysis Tools**: Screenshot of tools or dashboards used for deeper log analysis.
- **Token Experimentation**: Screenshot of different token types and their configurations.

## Conclusion & References
This project demonstrated the effectiveness of honeypots and Canary Tokens in detecting and analyzing malicious activities. By simulating vulnerabilities and tracking unauthorized access, valuable insights into attacker behaviors and tactics were gained.

### Suggested Screenshots:
- **Final Honeypot Report**: Screenshot of summarized honeypot findings.
- **Canary Token Summary**: Screenshot of triggered tokens and related alerts.

### References:
- [Cowrie Documentation](https://cowrie.readthedocs.io/en/latest/)
- [Canary Tokens](https://canarytokens.org/)
- [Best Practices for Honeypot Deployment](https://www.honeynet.org/)

