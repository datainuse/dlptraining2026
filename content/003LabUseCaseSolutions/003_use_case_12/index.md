---
title: "Use Case 12"
linkTitle: "Use Case 12"
weight: 12
---

{{% notice %}} Create an "incident notification" to send an email alert for any incident created with severity over 90

{{% /notice %}}

1. Click “Admin settings” in the left pane of the management console and click “Incident notifications.” Click “Create new subscription.”

    {{< figure src="case12_1.png" alt="case12_1" >}}

2. Enter an email address in the “Recipient” text box. Enable the “An incident is created” button and click “Create.”

    {{< figure src="case12_2.png" alt="case12_2" >}}

{{% notice tip%}}:bulb: Testing instructions:<br><br>
Make sure the policy group is published and that you have requested the new policy from the endpoint. To refresh the policy on the endpoint, navigate to:<br>

c:\program files\jazz networks\agent<br>

run the following command:<br>

agent config refresh<br>

Once you have refreshed the config, follow the below instructions to test the policy.

1. If you have completed configuration of all use cases prior to testing, there should already be a "Sequenced Incident" generated for your user under "Incidents" in the management console.
2. If you have been testing each use case individually as they are configured, perform the following actions to trigger the "Sequenced Incident"
   - Go to the "Management Console" and navigate to "Incidents"
   - Search for any "Sequenced Incidents" generated for your user name and resolve it/them
   - Perform the following steps to generate a new incident
   - Navigate to "dlptest.ai" and click "PDF" under "File Download"
   - Copy the file to the Desktop 
   - Navigate to "dlptest.ai" and upload the test file downloaded in step 2-1 above
   - The file upload should be blocked and a warning message displayed if "Use case 3" is configured correctly
3. A new "Sequenced Incident" should be created if "Use Case 11" has been configured correctly and an email should be sent to the configured email address
{{% /notice %}}