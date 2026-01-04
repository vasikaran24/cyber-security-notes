Analyzing DNS Log Files Using Splunk SIEM
------------------------------------------

Introduction
------------

Domain Name System (DNS) logs serve as an essential source of information for monitoring network behavior and identifying potential security threats. By leveraging the advanced analytical capabilities of Splunk Security Information and Event Management (SIEM), DNS log data can be systematically examined to detect anomalies, uncover indicators of compromise, and enhance overall situational awareness within the network environment

Project Overview
----------------
In this project, sample DNS (Domain Name System) log files will be ingested into the Splunk SIEM platform. Subsequent analysis will be conducted to extract meaningful insights regarding IP address allocation patterns, client activity, and overall network behavior

Prerequisites
-------------
Before analyzing DNS logs in Splunk, ensure the following:

Splunk instance is installed and configured.
DNS log data sources are configured to forward logs to Splunk.

Steps to Upload Sample DNS Log Files to Splunk SIEM
---------------------------------------------------

1. Prepare Sample DNS Log Files
--------------------------------

Obtain sample DNS log file in a suitable format (e.g., text files).
Ensure the log files contain relevant DNS events, including source IP, destination IP, domain name, query type, response code, etc.
Save the sample log files in a directory accessible by the Splunk instance.

2. Upload Log Files to Splunk
------------------------------

Log in to the Splunk web interface.
Navigate to Settings > Add Data.
Select Upload as the data input method.

3. Choose File
---------------
Click on Select File and choose the sample DNS log file you prepared earlier.

4. Set Source Type
------------------

In the Set Source Type section, specify the source type for the uploaded log file.
Choose the appropriate source type for DNS logs (e.g., dns or a custom source type if applicable).

5. Review Settings
------------------
Review other settings such as index, host, and sourcetype.
Ensure the settings are configured correctly to match the sample DNS log file.

6. Click Upload
----------------
Once all settings are configured, click on the Review button.
Review the settings one final time to ensure accuracy.
Click Submit to upload the sample DNS log file to Splunk

7. Verify Upload
-----------------
After uploading, navigate to the search bar in the Splunk interface.











