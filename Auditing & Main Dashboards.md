**Security Posture Overview**
![](assets/Pasted%20image%2020260903100803.png)

![](assets/Pasted%20image%2020260903101231.png)

![](assets/Pasted%20image%2020260903101251.png)![](assets/Pasted%20image%2020260903101257.png)



**Custom Insights**
- can get past the CID block by using these to grab the risks of all domains in totality
	- will not get nice UI, but will have all the data
	- can also do scheduled reporting for total risk evaluations



### Entity Business Card

**About Page**

![](assets/Pasted%20image%2020260903102159.png)


**Icons**
- briefcase = executive
	- C-Suite, BoS, etc
		- treated the same as privileged users



**Business Privileges**
- Settings > Miscellaneous Settings
- can add groups and set their impact accordingly

![](assets/Pasted%20image%2020260903102650.png)

- create CAP based on these privileges


**Activity**

![](assets/Pasted%20image%2020260903102936.png)
![](assets/Pasted%20image%2020260903102929.png)

**Risk**

![](assets/Pasted%20image%2020260903102843.png)


**Timeline**

![](assets/Pasted%20image%2020260903102914.png)


**Entity Pivots**

![](assets/Pasted%20image%2020260903103014.png)


The following increase sensitivity for the entity
- need to use these for better detections

![](assets/Pasted%20image%2020260903103042.png)

- marked entities drop after 48 hours
- watchlisted entities must be removed manually


**WHEN DOING AN INVESTIGATION**
- mark user right off the bat, could get more detections that way
	- they'll be removed from the watchlist automatically


**Users Dashboard**

![](assets/Pasted%20image%2020260903110442.png)


**Customizing Password Dictionary**
- any time that there is an account change and IdP is turned on, it'll do a hash assessment
	- partial hash assessment in the context of the password ONLY
	- account gets changed (migration, name change, etc)
	- pulled from HaveiBeenPwned - assessment done in CS cloud

Identity Protection > Inventory and Posture > Risk Configuration

![](assets/Pasted%20image%2020260903110647.png)


you can force a password check with FalconPy
- otherwise, it has to be an AD account change to check


**Analysis-Based Risk**
- don't remember seeing these in our environment, but here they are in their CID
	- can add exclusions as needed

![](assets/Pasted%20image%2020260903111506.png)

![](assets/Pasted%20image%2020260903111513.png)

![](assets/Pasted%20image%2020260903111522.png)

![](assets/Pasted%20image%2020260903111535.png)

![](assets/Pasted%20image%2020260903111540.png)


**User Accounts being Misclassified as Programmatic**
- when a migration happens and email gets wiped > moved to programmatic
- if they have an SPN > sometimes auto moved to programmatic
- can move them back by modifying the object


