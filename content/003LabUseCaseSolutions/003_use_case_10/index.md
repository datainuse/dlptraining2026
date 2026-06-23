---
title: "Use Case 10"
linkTitle: "Use Case 10"
weight: 10
---

{{% notice %}} Prevent a user from downloading and installing an unsafe application (7-zip.exe)

{{% /notice %}}

1. Open the policy group created in use case 2 (if not already open)

2. Click “Add policies” 

    {{< figure src="case10_1.png" alt="case10_1" >}}

3. Enter “download” into the “Search” text box OR expand “Browser templates” and select “Sensitive ZIP file downloaded”

   {{< figure src="case10_2.png" alt="case10_2" >}}

4. Change the policy name to “jsmith – Prevent download of unsafe file (7-zip.exe)” where “jsmith” is your first initial and last name.

5. Scroll to “File extensions” and click in “Select assets or define custom values”

   {{< figure src="case10_3.png" alt="case10_3" >}}

6. Select “Prohibit listed extensions” and enter the following extensions in the “Custom values” box one per line and click “Done”:</br>
    a. .exe</br>
    b. .msi</br>
    c. .tar</br>
    d. .xz</br>
    e. .dmg</br>
    e. .pkg

   {{< figure src="case10_4.png" alt="case10_4" >}}

7. Expand “Action configuration” and click to enable “Block browser download.” Next, enable “Display message. Enter “Use case 10” in the “Title” text box. Enter “Use case 10 – Prevent user from downloading unsafe files (7-zip.exe)” in the “Body” text box. Optionally, enable the other options in the “Display message” area if desired.

   {{< figure src="case10_5.png" alt="case10_5" >}}

8. Scroll down and click “Save and exit” in the lower right hand corner.

9. You should now see the newly created policy in the window

{{% notice tip%}}:bulb: Testing instructions:<br><br>
Make sure the policy group is published and that you have requested the new policy from the endpoint. To refresh the policy on the endpoint, navigate to:<br>

c:\program files\jazz networks\agent<br>

run the following command:<br>

agent config refresh<br>

Once you have refreshed the config, follow the below instructions to test the policy.

1. Navigate to "7-zip.org"
2. Click the link to download the .exe file for 64-bit x64 Windows
3. The file download should be prevented and a warning prompt displayed
{{% /notice %}}