![](assets/Pasted%20image%2020260903093915.png)

**Phone MFA is technically a fallback, on-screen is preferred**


### Authentication Traffic Inspection

**Identity Protection > Confiugre > Identity Configuration Policies**

![](assets/Pasted%20image%2020260903094140.png)

**Protocols and Active Directory Auditing**
- Identity Protection > Configure > Identity Configuration Policies

![](assets/Pasted%20image%2020260903094348.png)
- aggression level switch > if it's too noisy, try finding this
	- aggressive isn't best practice > good for pentests though


**Troubleshooting ATI Enablement**
![](assets/Pasted%20image%2020260903094917.png)



### What is a baseline?

**The Baseline: Your Context Clue**
- assessed within 21 days
- pulled from AD data
- user behavior

![](assets/Pasted%20image%2020260903095135.png)


**What does the baseline affect?**
- detections
	- "snapshot in time"
	- even if baseline is incomplete
- detections will still generate
- risks
	- will dynamically adjust over time



### Demo

**Identity Configuration Policies**

![](assets/Pasted%20image%2020260903095926.png)


**Default Policy**

![](assets/Pasted%20image%2020260903100015.png)
- enforcement mode still in beta

![](assets/Pasted%20image%2020260903100215.png)
- some settings require recent sensor versions


**Domain Status**
Identity Protection > Settings > Domain Controller Hosts

![](assets/Pasted%20image%2020260903100415.png)

