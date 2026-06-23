---
title: "Use Case 3"
linkTitle: "Use Case 3"
weight: 3
---

{{% notice %}} ### Prevent PII (US SSN) data from being uploaded to website

{{% /notice %}}

1. Open the policy group created in use case 2 (if not already open)

2. Click “Add policies”

    {{< figure src="case3_1.png" alt="case3_1" >}}

3. Enter “Upload” into the “Search” text box OR expand “Browser Templates” and select “Sensitive file uploaded”

    {{< figure src="case3_2.png" alt="case3_2" >}}

4. Change the policy name to “jsmith – Prevent upload of PII to website” where “jsmith” is your first initial and last name.

5. Scroll down to “Content inspection parameters” and click into “Select assets or define custom values”

   {{< figure src="case3_3.png" alt="case3_3" >}}

6. Enter “ssn” in the “Filter by policy asset name” and select “US Social Security Number (SSN)” by placing a check in the box. Click “Done” to finalize selection of the pattern.

   {{< figure src="case3_4.png" alt="case3_4" >}}

{{% notice tip%}} “Wide breadth detection” will match on the number only. “Narrow breadth detection” will match on the specified pattern in addition to a keyword as defined in the “Policy asset” being used. The test file downloaded from dlptest.ai will trigger the alert with either wide or narrow breadth selected.
{{% /notice %}}

7. Expand “Action configuration” and enable “Block browser upload” and “Display message. Enter “Use case 3” in the “Title” text box. Enter “Use case 3 – Block upload of PII to website” in the “Body” text box. Optionally, enable the other options in the “Display message” area if desired.

   {{< figure src="case3_5.png" alt="case3_5" >}}

8. Scroll down and click “Save and exit” in the lower right hand corner.

9. You should now see the newly created policy in the window

   {{< figure src="case3_6.png" alt="case3_6" >}}

{{% notice tip%}}:bulb: Testing instructions:<br><br>
Make sure the policy group is published and that you have requested the new policy from the endpoint. To refresh the policy on the endpoint, navigate to:<br>

c:\program files\jazz networks\agent<br>

run the following command:<br>

agent config refresh<br>

Once you have refreshed the config, follow the below instructions to test the policy.

1. Navigate to "dlptest.ai"
2. Click CSV under "File Download" to download a test file to the "Downloads" folder
3. Drag and drop the file downloaded in step two into the box under "File Upload"
4. File upload should be blocked and a prompt should appear on the screen.
{{% /notice %}}