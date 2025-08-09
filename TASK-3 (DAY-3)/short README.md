Step 1: Start GVM services
Opened a terminal in Kali Linux and ran:

sudo gvm-start
Waited for the services to start. The terminal displayed the web interface link: https://127.0.0.1:9392.

Step 2: Log in to Greenbone Security Assistant
Opened a web browser and navigated to https://127.0.0.1:9392.
Entered the username admin and the configured password to access the dashboard.

Step 3: Create a new scan target
Navigated to Scans → Targets → New Target in the Greenbone interface.
Entered:

Name: Localhost Scan

Hosts: 192.168.56.1
Saved the target.

Step 4: Create a new scan task
Went to Scans → Tasks → New Task.
Entered:

Name: Localhost Vulnerability Scan

Target: selected the target created in Step 3

Scan Config: Full and fast
Saved the task.

Step 5: Start the scan
Clicked the play button next to the new task to start the scan.
Allowed the scan to run until completion. A full scan typically takes 30–60 minutes.

Step 6: View scan results
Once the status changed to “Done,” clicked the task name to open the report.
Reviewed vulnerabilities categorized by severity: Critical, High, Medium, Low.
