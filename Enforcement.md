Dependent on access type
- general
	- On-prem
- cloud
	- Entra
- federated
	- ADFS

- on-screen MFA
	- requires RTR to be on to deliver that notification



**Actions**
- add to watchlist
	- greater scrutiny on an entity
- block
- identity verification (requires connector)
	- on-screen challeneges require the source endpoint have RTR enabled
	- mobile push as backup
	- notifications via Teams


**Simulation Mode and Audit**
- audit is its own action
	- no effect for end-user
	- can be used to create a custom detection
- simulation mode logged as the respective action
	- testing rules before deployment into prod



**Conditional Access Settings**
FalconID is the MFA tool that uses on-screen notifications

![](assets/Pasted%20image%2020260903133534.png)

- if rules don't seem to be working, check distribution status on the top right of the policies page - shows when policies were last enforced

**CAP Rules**
Policies follow firewall standard
- put broad rules on the bottom


**Analytics**

![](assets/Pasted%20image%2020260903133709.png)




**Setting up MFA**

FalconID needs TOTP Authenticator

![](assets/Pasted%20image%2020260903134923.png)

also need to check conditional access settings

![](assets/Pasted%20image%2020260903134940.png)

- change connector in the policy to the FalconID connector


MFA Prompt Settings
- best practice:
	- once a session is best
	- in context of user + source
		- verifies the user and their source endpoint > good for admins that remote into many machines

![](assets/Pasted%20image%2020260903135051.png)

- also enable the on-screen notification
![](assets/Pasted%20image%2020260903135814.png)

