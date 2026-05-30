# CVE-2024-3400
This program was improved upon to include a safety-feature which will catch the cases that will cause this script to be caught in indefinitely <br>

The base script was created by retkoussa and referenced [here](https://github.com/retkoussa/CVE-2024-3400/blob/main/main.py).<br>
Problem with the above script:- The script fails if the connection is reset by the Target Server --> Causing a Error.

What was changed:- Inserted a TRY/EXCEPT Block.<br>

How to Use? 
- If you are testing a bunch of Servers for this vulnerability --> They are most likely using Global-Protect VPN to authenticate using PAN-OS as a base.<br>
- Perform DNS Resolution and gather all the IP addresses. Put them on a single file. Ex.: ip_CVE-2024-3400.txt<br>
- Run this Python script using: `python3 CVE-2024-3400.py`
- When asked this, enter the filename as the argument: `Enter the file path containing IP addresses: ip_CVE-2024-3400.txt` 





