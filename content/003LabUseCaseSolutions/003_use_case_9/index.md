---
title: "Use Case 9"
linkTitle: "Use Case 9"
weight: 9
---

{{% notice %}} ### Generate a warning prompt for users visiting an AI website (chatgpt.com, etc.)
{{% /notice %}}

1. Open the policy group created in use case 2 (if not already open)

2. Click “Add policies” 

    {{< figure src="case9_1.png" alt="case9_1" >}}

3. Enter “Unauthorized website” into the “Search” text box OR expand “Browser templates” and select “Unauthorized website accessed”

   {{< figure src="case9_2.png" alt="case9_2" >}}

4. Change the policy name to “jsmith – Warn user when accessing AI website (chatgpt.com)” where “jsmith” is your first initial and last name.

5. Scroll to “Website parameters” and click in “Select assets or define filters”

   {{< figure src="case9_3.png" alt="case9_3" >}}

6. Click “Specify SaaS app conditions.” Select “Prohibit listed SaaS apps.” Turn on “Categories.” Click “Select categories” and choose “Artificial Intelligense.” Click “Done” to add the category to the policy.

   {{< figure src="case9_4.png" alt="case9_4" >}}

7. Expand “Action configuration” and enable “Display message. Enter “Use case 9” in the “Title” text box. Enter “Use case 9 – Warn user when accessing AI website (chatgpt.com)” in the “Body” text box. Optionally, enable the other options in the “Display message” area if desired.

   {{< figure src="case9_5.png" alt="case9_5" >}}

8. Scroll down and click “Save and exit” in the lower right hand corner.

9. You should now see the newly created policy in the window

{{% notice tip%}}:bulb: Testing instructions:<br><br>
Make sure the policy group is published and that you have requested the new policy from the endpoint. To refresh the policy on the endpoint, navigate to:<br>

c:\program files\jazz networks\agent<br>

run the following command:<br>

agent config refresh<br>

Once you have refreshed the config, follow the below instructions to test the policy.

1. Navigate to "chatgpt.com"
2. A warning prompt should be displayed
{{% /notice %}}