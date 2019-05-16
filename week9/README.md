# Project 7 - Setting Up a HoneyPot

1. HoneyPot Deployed:
 - Ubuntu - Dionaea with HTTP

2. Issues Encountered:
- Faced a lot of issues with VM deployment on GCP. Earlier I was using the ```f1-micro``` instance. However, the deployment and packages installation was very slow. Later, I switched to the ```g1-small``` instance type. This sped up the process.
- I was not able to see the login screen for the mhn-admin instance. Due to this, I got stuck at the honeypot deployment stage. After a lot of googling and help from the TPMs I figured out that I had to manually enable HTTP and HTTPS traffic for the admin VM. After I enabled these options, the actual honeypot deployment went smoothly.
- Steps: 
1. Go to GCP Console
2. Go to Compute and click on your mhn-admin VM instance
3. Click edit
4. Scroll down and enable HTTP and HTTPS

3. Summary of HoneyPot Data:
 - Total time HoneyPot is active: 30 minutes.
 - Total attacks: 1774
 - JSON Output file: Available in root folder
