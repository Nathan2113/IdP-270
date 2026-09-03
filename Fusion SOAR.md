**Basics of Workflows**

![](assets/Pasted%20image%2020260903142401.png)


**IDP and Fusion SOAR**
- can enrich data from different modules and throw them all into a case



**Use Case: Enriching Detections with EDR - SUPER IMPORTANT**
- grab cli history, find recent logins, retrieve executed processes, etc
	- be sure to use parallel processing

![](assets/Pasted%20image%2020260903142710.png)


**Example workflow**

![](assets/Pasted%20image%2020260903135906.png)


**Demo**
- use "from playbook" button to see what is possible
	- also check Fusion SOAR > Content Library


suspicious LDAP search condition

![](assets/Pasted%20image%2020260903143301.png)


another condition (gonna be a logical OR)

![](assets/Pasted%20image%2020260903143503.png)

- covers either eventuality - otherwise there could be some false negatives


add the user to watchlist, sleep 5 min, remove from watchlist

![](assets/Pasted%20image%2020260903143714.png)


enrich the detection with more data
- sequential action between enrichment and detection comment

![](assets/Pasted%20image%2020260903143757.png)
![](assets/Pasted%20image%2020260903143848.png)




**Exercise**

![](assets/Pasted%20image%2020260903141850.png)

![](assets/Pasted%20image%2020260903141857.png)

![](assets/Pasted%20image%2020260903141903.png)

![](assets/Pasted%20image%2020260903141908.png)

![](assets/Pasted%20image%2020260903141913.png)

![](assets/Pasted%20image%2020260903141918.png)