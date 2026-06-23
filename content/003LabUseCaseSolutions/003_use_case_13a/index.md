---
title: "Use Case 13A"
linkTitle: "Use Case 13A"
weight: 13
---

{{% notice %}} Prevent an unauthorized application from launching (calc.exe)

{{% /notice %}}

1. Open the policy group created in use case 2 (if not already open)

2. Click “Add policies” 

    {{< figure src="case13a_1.png" alt="case13a_1" >}}

3. Enter “unauthorized application” into the “Search” text box OR expand “External threat templates” and select “Unauthorized application used”

   {{< figure src="case13a_2.png" alt="case13a_2" >}}

4. Change the policy name to “jsmith – Prevent unauthorized application from launching (calc.exe)” where “jsmith” is your first initial and last name.

5. Scroll to “Application parameters” and select “Process parameters.” Click the text box under “Binary names” 

6. Select “Prohibit listed binaries.” Remove the existing entries from “Custom values” and enter “calc.exe”. Click “Done”

   {{< figure src="case13a_3.png" alt="case13a_3" >}}

7. Expand “Action configuration” and enable “Kill process” and “Display message.” Enter “Use case 13a” in the “Title” text box. Enter “Use case 13a – Prevent unauthorized application from launching (calc.exe)” in the “Body” text box. Optionally, enable the other options in the “Display message” area if desired.

   {{< figure src="case13a_4.png" alt="case13a_4" >}}

8. Scroll down and click “Save and exit” in the lower right hand corner.

{{% notice tip%}}:bulb: Testing instructions:<br><br>
Make sure the policy group is published and that you have requested the new policy from the endpoint. To refresh the policy on the endpoint, navigate to:<br>

c:\program files\jazz networks\agent<br>

run the following command:<br>

agent config refresh<br>

Once you have refreshed the config, follow the below instructions to test the policy.

1. Launch the "Calculator App" by typing "calc" into the Windows Search bar
2. Calculator should immediately be terminated and a warning prompt displayed
{{% /notice %}}