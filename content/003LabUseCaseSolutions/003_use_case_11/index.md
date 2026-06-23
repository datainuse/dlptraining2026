---
title: "Use Case 11"
linkTitle: "Use Case 11"
weight: 11
---

{{% notice %}} Create a "Sequenced Incident" for your device only

{{% /notice %}}

1. Click “Policies” in the left pane of the management console and select “Sequence rules” in the top center of the screen. Click “Create new rule.”

    {{< figure src="case11_1.png" alt="case11_1" >}}

2. Type “jsmith – Sequence detection rule” in the “Name” box and click “Next”

3. Select the following stages and click “Create”</br>
    a. Collection [TA0009]</br>
    b. Exfiltration [TA0010]

   {{< figure src="case11_2.png" alt="case11_2" >}}

4. Click the edit pencil in the “Include” box

   {{< figure src="case11_3.png" alt="case11_3" >}}

5. Select “Specific entities (by label)” and choose your label created in use case 1

   {{< figure src="case11_4.png" alt="case11_4" >}}

6. Click the edit pencil in the “Mandatory stages” box

   {{< figure src="case11_5.png" alt="case11_5" >}}

7. Select “Exfiltration [TA0010]” and click “Save”

   {{< figure src="case11_6.png" alt="case11_6" >}}

8. Click the drop down arrow in the "Risk score" box, choose "Fixed" and set to 100
   
   {{< figure src="case11_8.png" alt="case11_8" >}}

9. Click “Operation mode” and click “Enabled” then click “Publish rule”

   {{< figure src="case11_7.png" alt="case11_7" >}}

{{% notice tip%}}:bulb: Testing instructions:<br><br>
Make sure the policy group is published and that you have requested the new policy from the endpoint. To refresh the policy on the endpoint, navigate to:<br>

c:\program files\jazz networks\agent<br>

run the following command:<br>

agent config refresh<br>

Once you have refreshed the config, follow the below instructions to test the policy.

1. If you have completed configuration of all use cases prior to testing, there should already be a "Sequenced Incident" generated for your user under "Incidents" in the management console.
2. If you have been testing each use case individually as they are configured, perform the following actions to trigger the "Sequenced Incident"
   - Navigate to "dlptest.ai" and click "PDF" under "File Download"
   - Copy the file to the Desktop 
   - Navigate to "dlptest.ai" and upload the test file downloaded in step 2-1 above
   - The file upload should be blocked and a warning message displayed if "Use case 3" is configured correctly
3. Go to the Management Console and navigate to Incidents and look for your sequenced incident in the display
{{% /notice %}}