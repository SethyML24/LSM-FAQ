#lsmfaq #lsmguide

[[lsm_guide]]
[[MDR Architecture Diagram]]
# Sharepoint links

[Deployments Documentation](https://nclose365.sharepoint.com/:f:/r/sites/NviewResponseTeam-CustomerSuccess/Shared%20Documents/Customer%20Success/Deployment/Documentation?csf=1&web=1&e=Q5XkN9)

# **LSM FAQ**

**Please Note**

1. On the alert queue, always work from oldest to newest

2. On the alert queue, when you see a **Vsphere LSM** check on Kibana if logs are ingesting either via IP or FQDN(Google it)

	 You can check the IP address of any Vpshere LSM by utilizing the Messages Tab.

 **Stops ingesting via IP**
	 ![[FAQVpshere1.png]]

 **Starts ingesting via FQDN
	![[FAQVpshere2.png]]

	This is usually the case in the reverse order as well, when log stop ingesting
	via FQDN and start ingesting via IP instead.

3. When logging a git for LSM’s if dev/sysops tells you to mail client, do so in standard LSM alerting format

4. If an LSM case contains more than 4 host for the same index, use a spreadsheet to list hosts as shown below. Attach it to emails and refer to it in the relevant fields
	![[Spreadsheetdetails1.png]]

5. When asking question provide all the necessary information to make answering the question as easy as possible, example, relevant links & case numbers, etc.

6. Always message CS via slack when you need them to follow up with a client after 2 consecutive follow ups with no response from client, always give them the LSM case number.

7. Always check the relevant comms platforms, outlook, slack & github for any information on a specific **host/index & logsource** on open LSMs to assist in the remediation thereof. This includes previous cases sharing the same or similar details of any new open cases, previously logged gits and checking email threads and slack channels etc.

8. Do not share kibana links without a filter applied for 30 days or higher, you could risk slowing or breaking the cluster

9. When needing to escalate or request assistance on a case, please ensure that you include all relevant information on that case in your query, this includes links, case numbers & other relevant comms and information.

10. If not sure if something requires a git or mail check the following. Check the Meta Data tab on cyberfire, under Product/Data and Information in the Sources Tab
	![[CyberfireAPIInfor1 1.png]]

11. Also check on Github on the closed cases for log source missing.
	![[Cyberfiregit1.png]]

12. On cyberfire, please ensure that you include any relevant information for you cases In the notes and Description fields, this should include the following cyberfire details template as shown below.     
	1. ![[Cyberfiredetails template1.png]]

13. To find the engineer on LSM escalations for review in the current week, please check on the LSM deployments channel under the pinned tab.
	![[Pasted image 20250325155529.png]]

14. Always tag for reviews, if no one reviews your draft, tag them again
	 ![[Pasted image 20250325155956.png]]

15. Double check you links, mail and other details before posting an alert draft for review

16. When sending kibana links, make sure the relevant fields are tabled up. Example
**Tabled fields**
	![[Pasted image 20250325160528.png]]

**Un Tabled Fields**
	![[Pasted image 20250325160504.png]]

16. Please ensure you include any remediation details and follow the proper formatting for doing followups
	![[Pasted image 20250326150947.png]]
	
17. Please ensure you have you automatic signature setup for any mails you plan to send out

18. Before drafting for any Vivo Fortigate LSMs please check the weekly Vivo healtcheck mails being sent out for any offline firewalls

19. Review your fellow LSM teams drafts to the best of your abilities, please tag any seniors currently on escalation to confirm anything in the review process that you are uncertain about.

20. No need to @ someone if its a DM on slack

21.  If you aren't sure, ask someone, in the case of an LSM, best to ask a client to confirm instead of assuming

22.  

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
