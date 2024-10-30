# Installing Debian 12  on MAC OS Silicon M1 host using UTM

Download latest UTM app on https://mac.getutm.app/gallery/archlinux-arm click on download it should bring the app. 
Afer downloading select the browse UTM galerry to select the OS Version you need to install
<img width="888" alt="image" src="https://github.com/user-attachments/assets/4361e785-1b2a-45d1-8639-ee5140ab4037">

Right cilk the VM and click edit to bring the setting for disk and netwrok 
<img width="1286" alt="image" src="https://github.com/user-attachments/assets/c7227c78-6a27-474b-bd28-71cc71a31ee1">

Chnage network setting as following
<img width="835" alt="image" src="https://github.com/user-attachments/assets/5b08d3c9-d344-41da-bdaf-c63bb64d6ca5">


After adjusting the network and disk property  click on the  start button to start the virtual and do the ping to check network is working 
<img width="891" alt="image" src="https://github.com/user-attachments/assets/9024f4e6-e0ed-49a8-82ec-fb26f6a984e1">

<img width="823" alt="image" src="https://github.com/user-attachments/assets/f2e32363-bab3-4116-beaf-6781c5301810">


# Cyber kill Chain analysis summary
 Malicious users have targeted global networks from the beginning, initially through self-propagating code like viruses and worms.
 Advanced Persistent Threats (APTs), focused on data theft for economic or military gain, are now one of the largest risks, especially in certain industries.
 Traditional cybersecurity defenses like anti-virus and firewalls are insufficient against APTs, as they assume threats are automated and fixable.
 APT actors leverage sophisticated tools, zero-day exploits, and customized malware that traditional defenses can’t detect, maintaining prolonged access.
 To combat APTs, a "kill chain" framework is proposed to analyze and disrupt the sequential stages of an attack.
# Intelligence-driven Computer Network Defense
This strategy focuses on understanding adversaries—analyzing their capabilities, objectives, methods, and limitations—to address cyber risks effectively.
It involves a continuous process of using indicators from past intrusions to detect and analyze new threats, treating intrusions as multi-phase events rather than isolated incidents.
The kill chain model segments intrusions into phases, allowing defenders to disrupt any stage to thwart adversaries and prevent them from reaching their objectives
This model increases the cost and difficulty for attackers, showing that defenders, with proactive intelligence, can hold an advantage over persistent threats.

The kill chain model has been adapted for cybersecurity, where an attacker must progress through specific phases to achieve objectives within a targeted network.
Cyber Intrusion Phases: The cybersecurity kill chain has seven stages:

* Reconnaissance: Gathering information on targets.
* Weaponization: Creating a payload (e.g., malware).
* Delivery: Transmitting the payload via email, websites, or USB.
* Exploitation: Triggering the payload, often through vulnerabilities.
* Installation: Installing malware for continued access.
* Command and Control (C2): Establishing a communication channel to control the infected system.
* Actions on Objectives: Achieving goals like data theft or network infiltration.
* This model allows defenders to understand and disrupt each stage of an intrusion, preventing attackers from completing their objectives by intervening at any phase.

# Ep 138: The Mimics of Punjab Darknet Diaries

Full transcript can be found here https://darknetdiaries.com/transcript/138/
In this episode of darknet diaries scammers tried to use the phone channel to phone the victim acting as the relatives of the victim and get money out of them in favour of helping the family member. 

Tarun woke up one morning to missed calls from his cousin and sister. When he called his sister back, she was panicked and told him to speak to his cousin. Upon calling, Tarun’s cousin asked if he was okay, explaining that he had received a call from someone impersonating Tarun, claiming he was in jail and needed money. Concerned, his cousin had quickly sent money, assuming Tarun was in trouble.

Although Tarun wasn’t at fault, he decided to reimburse his cousin for the lost money. Reflecting on the incident, Jack noted that scams like these often target family members, playing on their instinct to help loved ones in distress. He highlighted the rise of AI-based scams that clone voices to make impersonation more believable. Tarun later saw similar scams circulating on social media, realizing his family wasn’t alone in experiencing this deception.


* MITRE ATT&CK FAQ is at https://attack.mitre.org/resources/faq/
* ATT&CK Enterprise Matrix is at https://attack.mitre.org/matrices/enterprise/
* Tactic refers to the overall reason that the attacker is trying to perform an action (technique), and answers the question "why". 
* In the ATT&CK Enterprise Matrix examples of tactics are e.g. Reconnaissance, Initial Access, Defence Evasion and Lateral Movement
* A technique and a sub-technique refers to a way an attacker could achieve the goals of a tactic. Examples include Active Scanning for the tactic Reconnaissance, Phishing and Supply Chain Compromise for the tactic Initial Access, Access Token Manipulation and Direct Volume Access for Defense Evasion and Exploitation of Remote Services for Lateral Movement
* A procedure is the specific implementation of a technique. For Active Scanning it could be a port scan to find open ports and services, for Phishing it could include crafting a legitimate-looking e-mail and linking it to a malicious website, and for Exploitation of Remote Services it could include using file shares to distribute malicious payloads across the network using shared credentials.
The matrix is relatively straightforward and the abstraction layers seem useful to group similar concepts into one. Even though a kill chain is not dependent on all tactics, a good cybersecurity posture should at the very least consider each of them and whether or not the various techniques should be (further) mitigated in the environment.









