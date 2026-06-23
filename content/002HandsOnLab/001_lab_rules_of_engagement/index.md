---
title: "Lab Rules of Engagement"
linkTitle: "Lab Rules of Engagement"
chapter: false
weight: 1
---

{{% notice warning %}} Please note that the FortiDLP management console is a shared environment. Any changes made can impact other users if not properly scoped via labels. Please see below before making any changes.{{% /notice %}}

{{% notice %}}:bulb: If you did not receive or cannot find the email with your login credentials, notify a course instructor who will initiate a "re-send" of the credentials.{{% /notice %}}

{{% notice %}}:bulb: When first created, all policy groups and configurations default to "All entities" in scope. Make sure to change the scope to your label ONLY! Failure to do so will impact other attendees' ability to test their configurations.<br><br> {{< figure src="lab_rules_1.jpg" alt="lab_rules_1" >}}{{% /notice %}}

{{% notice %}}:bulb: Use the following naming convention for all lab use cases and configurations: <br><br>
First initial followed by last name - use case (ex. Josh Smith creating a policy for use case 3 would be "jsmith - Prevent upload of PII to website").{{% /notice %}}

{{% notice %}}:bulb: It is recommended that you configure all use cases prior to testing them as some of the later use cases will automatically trigger during testing of earlier use cases if configured ahead of time. If you choose to test immediately, make sure that you publish the policy group. Once the policy group is published, refresh the policy on the endpoint by navigating to:<br>

c:\program files\jazz networks\agent<br>

run the following command:<br>

agent config refresh<br> <br><br>


{{% /notice %}}

{{% notice tip%}}:bulb: All use case solutions are available in the "Lab Use Case Solutions" page accessible via the course registration page. Please only view them if you are uncertain how to solve a problem.{{% /notice %}}