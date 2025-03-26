# **LSM FAQ**

# Sharepoint links
Please find the deployments documentation below.

[Deployments Documentation](https://nclose365.sharepoint.com/:f:/r/sites/NviewResponseTeam-CustomerSuccess/Shared%20Documents/Customer%20Success/Deployment/Documentation?csf=1&web=1&e=Q5XkN9)

[LSM Guide](https://nclose365.sharepoint.com/:f:/r/sites/NviewResponseTeam-CustomerSuccess/Shared%20Documents/Customer%20Success/Deployment/Documentation/LSM?csf=1&web=1&e=pi1Mzc)

**Frequently Asked Questions**

1. On the alert queue, always work from oldest to newest

2. On the alert queue, when you see a **Vsphere LSM** check on Kibana if logs are ingesting either via IP or FQDN(Google it)

	 You can check the IP address of any Vpshere LSM by utilizing the Messages Tab.

 **Stops ingesting via IP**
	![Alt text](https://github.com/SethyML24/LSM-FAQ/blob/main/LSMFAQ/Attachments/FAQVpshere1.png)

 **Starts ingesting via FQDN
 	![Alt text](https://github.com/SethyML24/LSM-FAQ/blob/main/LSMFAQ/Attachments/FAQVpshere2.png)

	This is usually the case in the reverse order as well, when log stop ingesting
	via FQDN and start ingesting via IP instead.

3. When logging a git for LSM’s if dev/sysops tells you to mail client, do so in standard LSM alerting format

4. If an LSM case contains more than 4 host for the same index, use a spreadsheet to list hosts as shown below. Attach it to emails and refer to it in the relevant fields
	
 ![Alt text](https://github.com/SethyML24/LSM-FAQ/blob/main/LSMFAQ/Attachments/Spreadsheetdetails1.png)

6. When asking question provide all the necessary information to make answering the question as easy as possible, example, relevant links & case numbers, etc.

7. Always message CS via slack when you need them to follow up with a client after 2 consecutive follow ups with no response from client, always give them the LSM case number.

8. Always check the relevant comms platforms, outlook, slack & github for any information on a specific **host/index & logsource** on open LSMs to assist in the remediation thereof. This includes previous cases sharing the same or similar details of any new open cases, previously logged gits and checking email threads and slack channels etc.

9. Do not share kibana links without a filter applied for 30 days or higher, you could risk slowing or breaking the cluster

10. When needing to escalate or request assistance on a case, please ensure that you include all relevant information on that case in your query, this includes links, case numbers & other relevant comms and information.

11. If not sure if something requires a git or mail check the following. Check the Meta Data tab on cyberfire, under Product/Data and Information in the Sources Tab
	![Alt text](https://github.com/SethyML24/LSM-FAQ/blob/main/LSMFAQ/Attachments/CyberfireAPIInfor1%201.png)

13. Also check on Github on the closed cases for log source missing.
	![Alt text](https://github.com/SethyML24/LSM-FAQ/blob/main/LSMFAQ/Attachments/Cyberfiregit1.png)

15. On cyberfire, please ensure that you include any relevant information for you cases In the notes and Description fields, this should include the following cyberfire details template as shown below.     
```
Kibana URL:
Log source:
Log type:
Last log:
Details: After reviewing the logs for the last 7 days we identified that logs stopped ingesting for this host.
```

16. To find the engineer on LSM escalations for review in the current week, please check on the LSM deployments channel under the pinned tab.
	![Alt text](https://github.com/SethyML24/LSM-FAQ/blob/main/LSMFAQ/Attachments/Pasted%20image%2020250325155529.png)

18. Always tag for reviews, if no one reviews your draft, tag them again
	![Alt text](https://github.com/SethyML24/LSM-FAQ/blob/main/LSMFAQ/Attachments/Pasted%20image%2020250325155956.png)

20. Double check your links, mails and other details before posting an alert draft for review

21. When sending kibana links, make sure the relevant fields are tabled up. Example
**Tabled fields**
	![Alt text](https://github.com/SethyML24/LSM-FAQ/blob/main/LSMFAQ/Attachments/Pasted%20image%2020250325160528.png)

**Un Tabled Fields**
 	![Alt text](https://github.com/SethyML24/LSM-FAQ/blob/main/LSMFAQ/Attachments/Pasted%20image%2020250325160504.png)

16. Please ensure you include any remediation details and follow the proper formatting for doing followups
	![Alt text](https://github.com/SethyML24/LSM-FAQ/blob/main/LSMFAQ/Attachments/Pasted%20image%2020250326150947.png)
	
18. Please ensure you have you automatic signature setup for any mails you plan to send out

19. Before drafting for any Vivo Fortigate LSMs please check the weekly Vivo healtcheck mails being sent out for any offline firewalls

20. Review your fellow LSM teams drafts to the best of your abilities, please tag any seniors currently on escalation to confirm anything in the review process that you are uncertain about.

21. No need to @ someone if its a DM on slack

22.  If you aren't sure, ask someone, in the case of an LSM, best to ask a client to confirm instead of assuming

23.  

# FYI
### Motuscorp

#### Known test servers
```
redhat8-img-clean.motus-corp-it.co.za
dhcp-map01.motus-corp-it.co.za
kea-stork.motus-corp-it.co.za
dhcp-map-01.motus-corp-it.co.za
dhcphq01.motus-corp-it.co.za
dhcp-imp-01.motus-corp-it.co.za
dhcp-ret-01.motus-corp-it.co.za
dhcp-map-02.motus-corp-it.co.za
kea-dhcp-ret01
bbc50.motus-corp-it-co-za
dhcp-ret-02.motus-corp-it.co.za
```

### Pragma
#### Known test servers
Anything containing *tst* for pragma is a potential test server
```
pra-tst-is-db1
pra-tst-is-fs1
pra-tst-is-kaf3
pra-tst-is-rep1
pra-tst-is-web3
pra-tst-is-kaf2
pra-tst-is-lb1
pra-tst-is-db2
pra-tst-is-kaf1
pra-tst-is-las1

lxacademy-staging2
lxacademy2
```



#### Authors
Kyle Hariparsaad
Seth Lackay
