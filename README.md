# Honeypot

Week 10/11

- Milestone 0: To The Cloud!
- Milestone 1: Create MHN Admin VM
- Milestone 2: Install the MHN Admin Application
- Milestone 3: Create a MHN Honeypot VM
- Milesotne 4: Install the Honeypot Application 
- Milestone 5: Attack!

Which Honeypot(s) Was Deployed:
- Dionaea with HTTP
- Wordpot
- p0f
- Snort

Issues Encountered: 
Accessing the admin console via the "superuser" values by loading the external IP in a browser proved to be an issue. When running the command "sudo supervisorctl status" there was an error with mhn-celery-worker which claimed to be fatal.

Attack Summary:

Top 5 Attacker IPs:
1. 61.160.215.38 (570 Attacks)
2. 35.225.81.112 (333 attacks)
3. 77.247.109.54 (178 attacks)
4. 180.168.46.118 (174 attacks)
5. 93.115.29.78 (88 attacks)

Top 5 Attacked Ports:
1. 80 (574 times)
2. 5060 (509 times)
3. 445 (285 times)
4. 1433 (191 times)
5. 8088 (164 times)

Top Honey Pots:
1. dionaea (2,954 attacks)
2. p0f (34 attacks)
3. snort (6 attacks)

Top Sensors:
1. mhn-honeypot-1 (2,961 attacks)
2. mhn-honeypot-3 (40 attacks)
3. mhn-honeypot-4 (6 attacks)

TOP Attack Signatures:
1. ET DROP Dshield Block Listed Source group 1 (4 times)
2. ET CINS Active Threat Intelligence Poor Reputation IP TCP group 81 (1 times)
3. ET CINS Active Threat Intelligence Poor Reputation IP TCP group 56 (1 times)
4. ET CINS Active Threat Intelligence Poor Reputation IP TCP group 49 (1 times)
5. ET SCAN Suspicious inbound to mySQL port 3306 (1 times)
