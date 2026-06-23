---
title: "Use Case 7"
linkTitle: "Use Case 7"
weight: 7
---

{{% notice %}} ### File downloaded from OneDrive Renamed
{{% /notice %}}

1. Open the policy group created in use case 2 (if not already open)

2. Click “Add policies”

    {{< figure src="case7_1.png" alt="case7_1" >}}

3. Enter “renamed” into the “Search” text box OR expand “File templates” and select “Sensitive file renamed”

    {{< figure src="case7_2.png" alt="case7_2" >}}

4. Change the policy name to “jsmith – File downloaded from OneDrive renamed” where “jsmith” is your first initial and last name.

5. Scroll down to “File origin parameters (Windows and macOS only)” and click into “Select assets or define filters”

    {{< figure src="case7_3.png" alt="case7_3" >}}

6. Click “Select from the SaaS app inventory”

    {{< figure src="case7_4.png" alt="case7_4" >}}

7. Click “Add Apps” in the upper right hand corner of the window

    {{< figure src="case7_5.png" alt="case7_5" >}}

8. Enter “one” into the “Filter by SaaS app name” text box and select “Microsoft 365 OneDrive” and “Microsoft OneDrive” by placing checks in the box. Click “Add apps”

    {{< figure src="case7_6.png" alt="case7_6" >}}

9. Click “Done” to add the apps to the policy

10. Scroll to “File action parameters” and ensure “Monitor file rename” is selected

    {{< figure src="case7_7.png" alt="case7_7" >}}

11. Scroll to “Content inspection parameters” and click “Select assets or define custom values”

12. Click the text box under “Custom Values” and enter “.*” in the box. Click “Done”

    {{< figure src="case7_8.png" alt="case7_8" >}}

 {{% notice tip%}} For “Sensitive file” policies, you must configure a value in the content inspection section. “.*” will match any content.
{{% /notice %}}

13. Scroll to and expand “Action configuration” and enable “Display message.” Enter “Use case 7” in the “Title” text box. Enter “Use case 7 – File downloaded from OneDrive renamed” in the “Body” text box. Optionally, enable the other options in the “Display message” area if desired.

    {{< figure src="case7_9.png" alt="case7_9" >}}

14. Scroll down and click “Save and exit” in the lower right hand corner.

15. You should now see the newly created policy in the window

{{% notice tip%}}:bulb: Testing instructions:<br><br>
Make sure the policy group is published and that you have requested the new policy from the endpoint. To refresh the policy on the endpoint, navigate to:<br>

c:\program files\jazz networks\agent<br>

run the following command:<br>

agent config refresh<br>

Once you have refreshed the config, follow the below instructions to test the policy.

1. Navigate to "https://login.microsoftonline.com/" and login using the credentials provided
2. Select "OneDrive" from the "App launcher" in the upper left hand corner of the web page
3. Download any file from any folder in OneDrive
4. If "Use case 5" has been completed and tested, the download should NOT be blocked, but a warning prompt should be displayed on the screen
5. Navigate to "dlptest.ai"
6. Go to the "Downloads" folder and rename the file downloaded in step 3
7. A warning prompt should be displayed
{{% /notice %}}
