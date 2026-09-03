**Identity Detections**
- based on a list of TTP's
- can include crossover data from other modules and third-party integrations
- snapshot in time severity set from the current baseline at the time of recording

![](assets/Pasted%20image%2020260903122250.png)


Identity detections can be queried in a CQL search as well
![](assets/Pasted%20image%2020260903122409.png)



**Detection Settings**
should NOT be turned on by default
- only turned on in specific use cases (i.e. pentest)

![](assets/Pasted%20image%2020260903122810.png)

- geolocation is NOT a global allowlist or blocklist
	- just for IdP detections
	- only on the country level


**Exclusions**

![](assets/Pasted%20image%2020260903123442.png)

- not every detections allows you to do they - they are simply on/off



**Cases**
incidents are completely gone from IdP - replaced with NG-SIEM cases instead

![](assets/Pasted%20image%2020260903123642.png)



### Investigating Suspicious Domain Replication and Brute Force Detections

- will often see password brute force and suspicious domain replication next to each other

![](assets/Pasted%20image%2020260903124856.png)


**Brute Force**
Investigate > Search for involved entities in Threat Hunter

![](assets/Pasted%20image%2020260903130045.png)

click actions to see authentication error codes
- i.e. PREAUTH_REQUIRED

![](assets/Pasted%20image%2020260903130127.png)


Investigate > Investigate Involved Endpoints
- will give you most the query already
- add `| "#event_simpleName" = ActiveDirectoryAuthenticationFailure` to get more info

EXAMPLE:
```
SourceEndpointHostName="GRUESOFT-CONT" OR SourceEndpointAccountObjectGuid="7903DE85-68D5-379B-A8E3-CE0DBB660C52" OR SourceEndpointAccountObjectGuid_readable="7903DE85-68D5-379B-A8E3-CE0DBB660C52"

| "#event_simpleName" = ActiveDirectoryAuthenticationFailure
```
![](assets/Pasted%20image%2020260903130250.png)

- gives more information than threat hunter will due to AD auditing


**Suspicious Domain Replication**
Source Endpoint > Host Search > Detections
- make sure to change time range

![](assets/Pasted%20image%2020260903130438.png)


can see unresolved detections here, in this example mimikatz.exe

![](assets/Pasted%20image%2020260903130554.png)

since we know it's mimikatz, go to Processes and Services > Process Executions
- in process executions, we can see the DCSync flag from mimikatz

![](assets/Pasted%20image%2020260903130744.png)

