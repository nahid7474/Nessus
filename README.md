Summary of this project:
---------------------------------------------------------------------------
In this project, I will perform vulnerability scans using Nessus Essentials on my Windows 10 virtual machine sitting on my Oracle VirtualBox.
This involves downloading and installing Nessus from the Tenable website, launch Nessus and access its web interface via localhost. 
Log in and configure a new scan by specifying targets and scan settings. Start the scan and monitor its progress. 
Once completed, I will will through scan results for identified vulnerabilities and then generate reports and finally take necessary actions to remediate vulnerabilities.
------------------------------------------------------------------------------------------------------------------------------------------------------------

Download and Install Nessus:
 
Firstly, I went to the Tenable website from my browser here https://www.tenable.com/products/nessus/nessus-essentials and sign up.
THen I downloaded the Nessus Essentials installer for my Windows 10 64bit machine.
Ran the installer and followed the on-screen instructions to install Nessus it.

<img src="https://github.com/nahid7474/Photos/blob/main/nessus.png"/> 

Once Nessus is installed, I launched the Nessus application by Opening my web browser and navigate to https://localhost:8834.
Clicked on the prompt "Connect via SSL"

<img src="https://github.com/nahid7474/Photos/blob/main/nessus2.png"/> 

Got the activation code using my business account and saved the activation code. 

<img src="https://github.com/nahid7474/Photos/blob/main/nessus3.png"/>

This has installed and configured all the requird plugins to run Nessus. Give it some time to finish this task.

<img src="https://github.com/nahid7474/Photos/blob/main/nessus4.png"/>

Once done, Nessus is ready to take on my target machine/netwok/website.
In this example, I will add my virtual machine's IP which is 10.0.2.15 and Nessus will find this host on the next window.
Now I will confugure the on demand scan to run.

<img src="https://github.com/nahid7474/Photos/blob/main/nessus5.png"/>



Configure Scanning:

I will configure two scans. 
First scan will only focus on open ports and associated vulnerabilities on my host 10.0.2.15
The second scan will do a more robust scan on the same machine. 

First Scan:
Click on the "Scans" tab in the top menu bar and then click on "New Scan" to create a new scan. Enter a name and optionally provide a description.
Choose the target as 10.0.2.15. Click on the "Launch" button to start the scan.


After the scan completes, click on the scan name to view the results, associted vulnerabilities.

Configure Second Scan: 
Click on the "Scans" tab in the top menu bar and then click on "New Scan".
Enter a name and optionally provide a description. THis time the type of the scan is basic network scan. Choose the target as 10.0.2.15. Click on the "Launch" button to start the scan.
Wait for some time to finish the scan. It took 26 minutes to finish the scan. 


Similar to the first scan, Nessus is showing the results, severity, CVSS score, remediations etc.


Generate Reports:

Nessus generates comprehensive reports summarizing the scan results. 
Here is the report I have produced for reference. <a href="https://github.com/nahid7474/Nessus/blob/main/Nessus%20Report.pdf">Nessus Report</a> 

Remediate Vulnerabilities:

I notice that the remediation action is: 
Security Updates for Microsoft .NET Framework (April 2024)

Now I will install the latest version of .NET Framework and then redo the scan to make sure the vulnerability is mitigated. 
