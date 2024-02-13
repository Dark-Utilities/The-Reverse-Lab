[Website Link](https://killbot.to/) | [Invoices Database](https://github.com/Dark-Utilities/The-Reverse-Lab/raw/main/Websites/killbot.to/data/invoices.log) | [Excalidraw Schema](https://excalidraw.com/#json=79Jut7m8EwtS9lufYmpxm,Jm0mHGf9gjSVqvs4bK0buQ)
### Monikers
  The moniker is french (**213.56.129.110** France, Paris), he is working alone and seem to not be part of a known APT.

### Description
Killbot.to presents itself as a service ostensibly designed to protect websites from being flagged by web browsers' security systems, particularly those that issue red page alerts for potentially malicious or harmful content. However, beneath its facade of legitimacy lies a darker truth: Killbot.to serves as a facilitator for scammers and fraudulent actors, providing them with a means to evade detection and continue their illicit activities unhindered.

Operating under the guise of a legitimate service, Killbot.to employs techniques to block crawlers and bots that are commonly used by web browsers to identify and flag malicious websites. By effectively circumventing these detection mechanisms, the service enables scammers to maintain their phishing pages without triggering the warning signals that would typically deter unsuspecting users from falling victim to their schemes.

Despite presenting itself as a solution for website owners seeking to enhance their online security, Killbot.to's true nature as a tool for enabling deception and fraud becomes evident upon closer examination. Rather than serving the interests of legitimate businesses or individuals, it actively aids and abets those engaged in malicious activities, thereby perpetuating harm within the online ecosystem.

The deceptive practices employed by Killbot.to highlight the ongoing challenges faced in combating online fraud and cybercrime. While efforts to enhance web security and protect users from malicious threats are continually evolving, the existence of services like Killbot.to underscores the need for vigilance and skepticism when navigating the digital landscape.

In conclusion, Killbot.to represents a disturbing example of how deceptive services can exploit vulnerabilities in online security systems to facilitate fraudulent activities. By masquerading as a legitimate solution while enabling malicious behavior, it undermines trust in the integrity of the online environment and underscores the importance of robust security measures and user education in combating cybercrime.

### Investigation's result
#### plisio.net gateway's transcation's database:
Based on our investigation, we have uncovered concerning evidence linking Killbot.to to fraudulent activities. 
Firstly, we have identified a list of invoices containing cryptocurrency addresses belonging to customers. 
These invoices suggest a financial transactional relationship between Killbot.to and individuals engaging in potentially illicit activities.
![image](https://github.com/Dark-Utilities/The-Reverse-Lab/assets/69421356/ef5b28fe-16f2-45f8-a834-c54cf2a29b7c)

### Telegram advertising
Additionally, we have obtained screenshots showing the owners of Killbot.to advertising their services on a Telegram channel known for promoting scamming activities. 
This direct association with known scammers further corroborates our suspicions regarding the true nature of Killbot.to's operations.
![image](https://github.com/Dark-Utilities/The-Reverse-Lab/assets/69421356/c2018d0e-c2e4-4e1c-8e18-d72b4008f2de)

### Backend infrastructure
During our investigation, we successfully traced the backend infrastructure of Killbot.to, revealing a complex network of servers used to host and operate the service. The path from the Killbot.to domain to its backend servers involves multiple layers of infrastructure.
Initially, requests to Killbot.to are proxied through Cloudflare, a popular content delivery network and DDoS protection service. Cloudflare obscures the origin server's IP address, making it more difficult to directly identify the physical location and hosting provider of the backend servers.
However, through thorough analysis and monitoring of network traffic, we were able to identify the actual IP addresses of the backend servers. The backend servers are hosted in two distinct locations:
  - (1) 178.208.92.111 (Russia, AS210079): This IP address serves as an intermediary between Cloudflare and the final backend server. It is registered to a hosting provider in Russia, indicating a potential physical location for part of Killbot.to's infrastructure.
  - (2) 213.56.129.110 (France, AS3215): This IP address represents the final backend server that handles requests from Cloudflare and executes the functionality of Killbot.to. It is hosted by a provider in France, suggesting another geographic location for part of the service's infrastructure.

The use of servers in different countries adds another layer of complexity to the investigation and may be indicative of efforts to obfuscate the true origin of Killbot.to's operations. However, our ability to uncover and trace the backend IPs demonstrates our commitment to uncovering the truth behind fraudulent activities and holding those responsible accountable for their actions.
![image](https://github.com/Dark-Utilities/The-Reverse-Lab/assets/69421356/e4a08797-b28f-434d-8f8b-e30ed319f40b)
<br>
Moving forward, further analysis of these IP addresses and collaboration with relevant authorities may be necessary to dismantle Killbot.to's infrastructure and disrupt its ability to facilitate online fraud.

#### Phishing pages hosting service
In addition to the backend infrastructure described earlier, our investigation has unveiled another significant aspect of Killbot.to's operations: the utilization of an Amazon Web Services (AWS) server for hosting phishing pages. This server, configured with Plesk control panel software, represents a separate component of Killbot.to's infrastructure dedicated specifically to the deployment of deceptive and fraudulent content.
![18 193 70 160_explore](https://github.com/Dark-Utilities/The-Reverse-Lab/assets/69421356/f02a1938-9970-4781-877b-78919e5d2c83)

#### Package attached to their project
The site refers to an npm killbot.to package whose author is "~killbot.to", we learn from the source of the package on github that the github account that worked on it forked a project called "killbot.pw" which belongs to a certain "mr-giovany".
![image](https://github.com/Dark-Utilities/The-Reverse-Lab/assets/48413426/80cca5d7-9b4e-466f-a752-010dd9f0dcfa)

#### Source Template Admin Panel
![image](https://github.com/Dark-Utilities/The-Reverse-Lab/assets/48413426/204b37bd-a93e-42e8-8801-eb1a101ba584)
![image](https://github.com/Dark-Utilities/The-Reverse-Lab/assets/48413426/a2731c81-67cc-44d5-be36-8283d6c8c37a)
![image](https://github.com/Dark-Utilities/The-Reverse-Lab/assets/48413426/e2d7754d-29af-47dc-86b1-bebb1e573a87)
<br>
The template used by killBot.to is Volt Bootstrap.
