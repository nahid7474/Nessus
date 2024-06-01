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

Click on the "Scans" tab in the top menu bar and then click on "New Scan" to create a new scan.
Enter a name for your scan and optionally provide a description.
Choose the target for your scan. You can specify individual IP addresses, ranges, or hostnames.
Configure other scan settings such as scan type (e.g., Basic Network Scan, Web Application Tests), scan policy (e.g., Basic Network Scan, Web Application Tests), and schedule (if needed).
Start the Scan:

After configuring the scan settings, click on the "Launch" button to start the scan.
Monitor Scan Progress:

Once the scan is launched, you can monitor its progress in the "Scans" tab. Nessus will display information such as the current status, number of hosts scanned, vulnerabilities found, etc.
Review Scan Results:

After the scan completes, click on the scan name to view the detailed results.
Nessus will provide a list of vulnerabilities found, along with severity ratings, affected hosts, and potential remediation steps.
You can filter and sort the results to focus on specific vulnerabilities or hosts.
Generate Reports:

Nessus allows you to generate comprehensive reports summarizing the scan results. You can customize the report format, content, and distribution options according to your needs.
Remediate Vulnerabilities:

Once you've reviewed the scan results, take appropriate actions to remediate the identified vulnerabilities. This may involve applying patches, updating software, or implementing configuration changes.
