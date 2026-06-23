---
title: "Use Case 5"
linkTitle: "Use Case 5"
weight: 5
---

{{% notice %}} ### Generate a warning prompt for any file downloaded from OneDrive

{{% /notice %}}


1. Open the policy group created in use case 2 (if not already open)

2. Click “Add policies”

    {{< figure src="case5_1.png" alt="case5_1" >}}

3. Enter “download” into the “Search” text box OR expand “Browser templates” and select “Sensitive file downloaded”

    {{< figure src="case5_2.png" alt="case5_2" >}}

4. Change the policy name to “jsmith – Warn any file downloaded from OneDrive” where “jsmith” is your first initial and last name.

5. Scroll down to “Website Parameters” and click into “Select assets or define filters” under “SaaS apps”

   {{< figure src="case5_3.png" alt="case5_3" >}}

6. Click “Select from the SaaS app inventory”

   {{< figure src="case5_4.png" alt="case5_4" >}}

7. Change the radio button to “Prohibit listed SaaS apps” and click “Add apps”

   {{< figure src="case5_5.png" alt="case5_5" >}}

8. Enter “one” into the “Filter by SaaS app name” text box and select “Microsoft 365 OneDrive” and “Microsoft OneDrive” by placing checks in the box. Click “Add apps”

   {{< figure src="case5_6.png" alt="case5_6" >}}

9. Click “Done” to add the apps to the policy

   {{< figure src="case5_7.png" alt="case5_7" >}}

10. Expand “Action configuration” and enable “Display message. Enter “Use case 5” in the “Title” text box. Enter “Use case 5 – Warn any file downloaded from OneDrive” in the “Body” text box. Optionally, enable the other options in the “Display message” area if desired.

   {{< figure src="case5_8.png" alt="case5_8" >}}

11. Scroll down and click “Save and exit” in the lower right hand corner.

12. You should now see the newly created policy in the window

{{% notice tip%}}:bulb: Testing instructions:<br><br>
Make sure the policy group is published and that you have requested the new policy from the endpoint. To refresh the policy on the endpoint, navigate to:<br>

c:\program files\jazz networks\agent<br>

run the following command:<br>

agent config refresh<br>

Once you have refreshed the config, follow the below instructions to test the policy.

1. Navigate to "https://login.microsoftonline.com/" and login using the credentials provided
2. Select "OneDrive" from the "App launcher" in the upper left hand corner of the web page
3. Download any file from any folder in OneDrive
4. The download should NOT be blocked, but a warning prompt should be displayed on the screen
{{% /notice %}}
