---
title: "Lab Access Instructions"
linkTitle: "Lab Access Instructions"
weight: 2
---

### Virtual Endpoint Access Instructions

1)	Enter the URL for your specific assigned VM device.

2)	Enter your assigned “username” and “password” in the appropriate fields and click "Login". The Username identifies your device:
  
    {{< figure src="vm_access_1.jpg" alt="labAccess1" >}}

{{% notice note %}} If you did not receive or cannot find the email with your login credentials, notify a course instructor who will assist you. {{% /notice %}}

### Management Console Access and Initial Configuration Instructions

{{% notice warning %}} Please note that the FortiDLP management console is a shared environment. Any changes made can impact other users if not properly scoped via labels. Please see the "Lab Rules of Engagement" page before making any changes.{{% /notice %}}

1)  Open your Chrome Browser on the virtual endpoint and navigate to the below URL:

https://fortidlp-training.reveal.nextdlp.com/

2)  Login to FortiDLP with the course credentials you received via the email address you used to register for the course.

    {{< figure src="vm_access_3.jpg" alt="consoleAccess1" >}}

{{% notice note %}} If you did not receive or cannot find the email with your login credentials, notify a course instructor who will initiate a "re-send" of the credentials. {{% /notice %}}

{{% notice tip %}} Your user name is your first initial followed by your last name... NOT your email address (ex. John Smith would be "jsmith") {{% /notice %}}

3)	Click the "Admin" icon:

    {{< figure src="vm_access_4.jpg" alt="labAccess4" >}}

4)	On Admin page click “Agent Deployment” in the left hand pane:

    {{< figure src="vm_access_5.jpg" alt="labAccess5" >}}

5)  Expand the "XPERTS2025" enrollment code and click "Copy code" then click "Download" to obtain the agent installer:

    {{< figure src="vm_access_10.jpg" alt="labAccess10" >}}

6)  Go to "Downloads" folder and double click the agent installer package downloaded in the previous step

7) Accept the terms in the license agreement and click "Next:"

    {{< figure src="vm_access_13.jpg" alt="labAccess13" >}}

8) Paste the enrollment code copied in step 5 into the text box under "Install with a code" and click "Install:"

    {{< figure src="vm_access_15.jpg" alt="labAccess15" >}}

9) When prompted, click "Finish" to complete the install:

{{% notice warning %}} When prompted, DO NOT reboot the machine at this point! {{% /notice%}}

10) Click "Nodes" in the left pane of the management console and click "Table" to confirm that your agent is reporting in successfully:

    {{< figure src="vm_access_18.jpg" alt="labAccess18" >}}

    {{< figure src="vm_access_19.jpg" alt="labAccess19" >}}

11) Reboot your VM and log in again.

12) CONGRATULATIONS! You have successfully installed the FortiDLP agent on your lab virtual machine.