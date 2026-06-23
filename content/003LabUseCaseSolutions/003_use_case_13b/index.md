---
title: "Use Case 13B"
linkTitle: "Use Case 13B"
weight: 14
---

{{% notice %}} Create a custom regular expression policy asset to match a number in the format: AA-111111

{{% /notice %}}

1. Click “Policies” in the left hand panel, click “Policy assets”, and click “Create new policy asset”

   {{< figure src="case13b_1.png" alt="case13b_1" >}}

2. Click in the text box for “Policy asset name” and enter “jsmith – use case 13b regex” where jsmith is your first initial followed by last name. Click “Generic string list” and select “Content inspection pattern.” Click the text box under “Name” and enter “jsmith - use case 13b regex”. Click in the text box under “Pattern” and enter “[a-zA-Z]{2}-\d{6}”. Click “Create.”

   {{< figure src="case13b_2.png" alt="case13b_2" >}}