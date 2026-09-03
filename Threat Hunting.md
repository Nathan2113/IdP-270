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
- mark user right off the bat, could find more detections that way
	- they'll be removed from the watchlist automatically

**User Accounts being Misclassified as Programmatic**
- when a migration happens and email gets wiped > moved to programmatic
- if they have an SPN > sometimes auto moved to programmatic
- can move them back by modifying the object