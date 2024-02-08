![Download Binary](ipfs://bafybeibq3l5mvr3ccotvnyfznl7ookmsadbkbor6t3apkvbo37rjcmwr24) | [Hashes](https://github.com/Inplex-sys/the-reverse-lab/blob/main/DataEyes.exe/HASHES)

### Monikers
  The origin of the attack seems to be a user called **leaksru** 🤡, this person doesn't seem to have mastered hacking and isn't part of any APT,
  the malware that is used is not developed by him and seem to be a public source.

### Description
This malware masquerading as malware-generating software, but in reality it steal credentials from users' browsers, Discord, and Telegram accounts. It operates by utilizing a Telegram bot to exfiltrate the stolen credentials. The malware itself is crafted using the Python programming language and compiled into an executable using PyInstaller. Additionally, the Python source file is encrypted using the AES encryption algorithm, likely to evade detection by security measures.

Upon execution, the malware likely performs the following actions:
  - Credential Theft: The malware actively monitors the user's browser, Discord, and Telegram applications for login credentials. It likely achieves this by intercepting network traffic or accessing stored credentials on the victim's system.

  - Communication with Telegram Bot: Once credentials are obtained, the malware communicates with a Telegram bot, likely hosted on the Telegram platform. It sends the stolen credentials to this bot for further processing or storage.
![image](https://github.com/Inplex-sys/the-reverse-lab/assets/69421356/b8f9f2a7-ed7a-434d-93f9-4bb09bc64416)

  - Encryption: The Python source file of the malware is encrypted using the AES encryption algorithm. This encryption serves to obfuscate the code and make analysis and detection more challenging for security researchers and antivirus solutions.
![image](https://github.com/Inplex-sys/the-reverse-lab/assets/69421356/3e4ef4ca-2c5a-4070-919a-a6fd470b8a83)


  - Persistence and Autostart: The malware may implement techniques to ensure persistence on the infected system, such as adding itself to startup items or modifying system settings. This ensures that the malware continues to operate even after system reboots.

  - Potential Additional Capabilities: While the primary function of the malware appears to be credential theft, it may also possess other malicious functionalities, such as keylogging, remote access, or further propagation mechanisms.
