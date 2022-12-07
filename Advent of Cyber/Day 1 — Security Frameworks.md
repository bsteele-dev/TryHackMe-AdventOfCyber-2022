# Day 1

## Security Frameworks

Documented processes that define policies and procedures organisations should follow to establish and manage security controls. They are blueprints for identifying and managing the risks they may face and the weaknesses in place that may lead to an attack.

### NIST Cybersecurity Framework
The framework focuses on five essential functions: 
`Identify` -> `Protect` -> `Detect` -> `Respond` -> `Recover` 

With these functions, the framework allows organisations to prioritise their cybersecurity investments and engage in continuous improvement towards a target cybersecurity profile.

### ISO 27000 Series
The ISO 27001 and 27002 standards are commonly known for cybersecurity and outline the requirements and procedures for creating, implementing and managing an information security management system (ISMS).

### MITRE ATT&CK Framework
A knowledge base of TTPs (Tactics, **T**echniques and Procedures) carefully curated and detailed to ensure security teams can identify attack patterns and develop effective security programs for their organisations. 


### Cyber Kill Chain
Describes the structure of an attack and consists of target identification, decision and order to attack the target, and finally, target destruction.

There are seven stages outlined by the Cyber Kill Chain, enhancing visibility and understanding of an adversary’s tactics, techniques and procedures.

![Image showcasing the seven steps of the Cyber Kill Chain.](https://tryhackme-images.s3.amazonaws.com/user-uploads/5fc2847e1bbebc03aa89fbf2/room-content/1e0cdd3b3f3c33c18d67f25aad84e618.png)


### Unified Kill Chain
Unification of the MITRE ATT&CK and Cyber Kill Chain frameworks.

The UKC provides a model to defend against cyber attacks from the adversary’s perspective. The UKC offers security teams a blueprint for analysing and comparing threat intelligence concerning the adversarial mode of working.

The Unified Kill Chain describes 18 phases of attack based on Tactics, Techniques and Procedures (TTPs).

#### CYCLE 1: In
The main focus of this series of phases is for an attacker to gain access to a system or networked environment. Typically, cyber-attacks are initiated by an external attacker. The critical steps they would follow are:

-   **Reconnaissance**: The attacker performs research on the target using publicly available information.
-   **Weaponisation**: Setting up the needed infrastructure to host the command and control centre (C2) is crucial in executing attacks.
-   **Delivery**: Payloads are malicious instruments delivered to the target through numerous means, such as email phishing and supply chain attacks.
-   **Social Engineering**: The attacker will trick their target into performing untrusted and unsafe action against the payload they just delivered, often making their message appear to come from a trusted in-house source.
-   **Exploitation**: If the attacker finds an existing vulnerability, a software or hardware weakness, in the network assets, they may use this to trigger their payload.
-   **Persistence**: The attacker will leave behind a fallback presence on the network or asset to make sure they have a point of access to their target.
-   **Defence Evasion**: The attacker must remain anonymous throughout their exploits by disabling and avoiding any security defence mechanisms enabled, including deleting evidence of their presence.
-   **Command & Control**: Remember the infrastructure that the attacker prepared? A communication channel between the compromised system and the attacker’s infrastructure is established across the internet.

This phase may be considered a loop as the attacker may be forced to change tactics or modify techniques if one fails to provide an entrance into the network.


#### CYCLE 2: Through
Attackers will be interested in gaining more access and privileges to assets within the network.

The attacker may repeat this phase until the desired access is obtained.

* **Pivoting**: Remember the system that the attacker may use for persistence? This system will become the attack launchpad for other systems in the network.
-   **Discovery**: The attacker will seek to gather as much information about the compromised system, such as available users and data. Alternatively, they may remotely discover vulnerabilities and assets within the network. This opens the way for the next phase.
-   **Privilege Escalation**: Restricted access prevents the attacker from executing their mission. Therefore, they will seek higher privileges on the compromised systems by exploiting identified vulnerabilities or misconfigurations.
-   **Execution**: With elevated privileges, malicious code may be downloaded and executed to extract sensitive information or cause further havoc on the system.
-   **Credential Access**: Part of the extracted sensitive information would include login credentials stored in the hard disk or memory. This provides the attacker with more firepower for their attacks.
-   **Lateral Movement**: Using the extracted credentials, the attacker may move around different systems or data storages within the network, for example, within a single department


#### CYCLE 3: Out
The Confidentiality, Integrity and Availability (CIA) of assets or services are compromised during this phase.

* **Collection**: After finding the jackpot of data and information, the attacker will seek to aggregate all they need. By doing so, the assets’ confidentiality would be compromised entirely, especially when dealing with trade secrets and financial or personally identifiable information (PII) that is to be secured.
-   **Exfiltration**: The attacker must get his loot out of the network. Various techniques may be used to ensure they have achieved their objectives without triggering suspicion.
-   **Impact**: When compromising the availability or integrity of an asset or information, the attacker will use all the acquired privileges to manipulate, interrupt and sabotage. Imagine the reputation, financial and social damage an organisation would have to recover from.
-   **Objectives**: Attackers may have other goals to achieve that may affect the social or technical landscape that their targets operate within. Defining and understanding these objectives tends to help security teams familiarise themselves with adversarial attack tools and conduct risk assessments to defend their assets.