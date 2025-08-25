# Kittengram-A-B-Test-Results-
This project investigates the impact of introducing sponsored, relevant ads on the Kittengram social media platform.

The analysis uses a simulated dataset to evaluate the effect on key user engagement metrics, specifically **Click-Through Rate (CTR)** and **Daily Active Users (DAU)**, through an A/B test. The primary goal is to determine if tailored ads can increase user engagement without negatively affecting user retention.

## Business Problem

Kittengram is a social media app for cat lovers, with a business model based on advertising. Currently, the generic ads shown to users are not relevant, leading to low engagement. A major cat product retailer, 'Kitten Zone', has proposed sponsoring posts with affiliate links. The hypothesis is that these more relevant, tailored ads will increase user engagement. This project aims to validate this hypothesis and provide data-driven recommendations.


## Dataset

The dataset used for this analysis was programmatically **generated to simulate user activity** on the Kittengram app. It includes three main tables, with key variables such as:

* **`dt`**: The date of the event.
* **`userid`**: A unique user identifier.
* **`activity_level`**: A numeric value representing a user's daily activity.
* **`ctr`**: The daily click-through rate for each user.


## Key Metrics and Methodology

The A/B test was designed to compare a **control group** (seeing generic ads) against a **test group** (seeing sponsored, relevant ads).

* **Success Metric**: **Click-Through Rate (CTR)**. We hypothesize that relevant ads will lead to a higher CTR.
* **Guardrail Metric**: **Daily Active Users (DAU)**. We must ensure the new ads do not cause a drop in the number of active users, which would indicate a negative user experience.

A binomial sample size calculation was performed to ensure the test had sufficient power to detect a significant effect.

<img width="704" height="489" alt="visualization" src="https://github.com/user-attachments/assets/b2f85606-89d2-4025-a939-4e22515ada85" />


## Key Findings

Based on the A/B test results, we observed a significant impact on both key metrics:

* **CTR:** The test group's CTR was **significantly higher** than the control group's CTR during the test period. This supports our hypothesis that tailored ads are more engaging for users.
* **DAU:** The test group showed a **drastic and sustained increase** in Daily Active Users compared to the control group, which remained stable. This suggests that the relevant ads not only drove clicks but also increased overall user activity.

## Recommendations

1.  **Proceed with Ad Launch**: The A/B test strongly suggests that sponsored posts from 'Kitten Zone' are effective. The significant increase in CTR and a positive (though simulated) impact on DAU indicate this is a beneficial change for both user engagement and potential revenue.

2.  **Monitor in Production**: Given the generated nature of the dataset, it is critical to implement a robust monitoring system for both CTR and DAU after the feature's full launch. This will confirm if the positive results are replicated in a real-world environment.


