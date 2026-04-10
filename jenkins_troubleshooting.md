# Jenkins troubleshooting

## Issue: 
- After briefly shutting down my Jenkins EC2 instance and powering it back on, when I try to navigate to different sections of Jenkins, it takes at least a minute to get to its destination.

## Solution: 
- This is caused by your EC2 generating a new public IP address upon launching after being powered off.

![ec2 pic of public ip address](./images/.png)

- First, verify that your Jenkins instance's current URL matches the Jenkins URL within the Jenkins console's system settings.

![jenkins homepage pic](./images/.png)

- On the Jenkins homepage, click the gear icon to get to the Jenkins settings page.

![Click the gear icon pic](./images/.png)

- Within the Settings page, click System.

![jenkins system pic](./images/.png)

- Once in System settings, scroll down to the Jenkins Location section.

![jenkins location section pic](./images/.png)

- Under the Jenkins Location section, access the Jenkins URL field and verify that the IP address within the field matches the IP address within your browser's address bar. 

![jenkins url field pic](./images/.png)

- If they do not match, replace the Jenkins URL with the current Jenkins IP address.

![jenkins url and jenkins url field pic](./images/.png)

- Scroll to the bottom of the page and click Apply then Save.

![apply and save button pic](./images/.png)

- The transition back to the Systems settings page should be immediate and proof that the issue is resolved.

![page transition gif](./images/.gif)

- Done.  


	
