# A/B Test Analysis of a New User Onboarding Campaign

## Business Context

A subscription-based digital product company introduced a new onboarding and activation campaign to improve user conversion and early engagement. To evaluate the effectiveness of the new onboarding experience, an A/B experiment was conducted in which users were randomly assigned to either the existing onboarding process (Control group) or the new onboarding campaign (Treatment group).

The objective of this analysis is to determine whether the treatment should be launched to all users based on statistical evidence and business performance metrics.

---

## Business Problem

The primary business decision is whether the new onboarding campaign should replace the existing onboarding experience.

This decision impacts:

* Product Management
* Marketing Team
* Customer Success Team
* Company Leadership
* Current and Future Users

The primary metric expected to improve is the **Paid Conversion Rate**. However, the decision should also consider potential risks such as higher refund rates, increased support tickets, lower engagement, or poor performance within specific user segments.

A recommendation should only be made after evaluating statistical significance, business metrics, guardrail metrics, and segment-level performance.

---

## Dataset Description

The dataset contains user-level information collected during the A/B experiment.

Each record represents one user and includes information such as:

* Experiment group (Control or Treatment)
* Landing page visit
* Trial start status
* Onboarding completion
* Paid conversion
* Revenue generated
* Refund requests
* Support tickets
* Engagement score
* Days to convert
* Region
* Device type
* Traffic source
* Subscription plan

The dataset was used to compare business performance between the control and treatment groups.

---

# North Star Metric

**Paid Conversion Rate**

Paid Conversion Rate measures the percentage of users who convert from free users to paying subscribers.

Formula:

Paid Conversion Rate = Converted Users ÷ Total Users

This metric directly reflects the business objective of increasing subscription revenue.

---

# KPI Tree Summary

Business Goal:
Increase Subscription Revenue

North Star Metric:

* Paid Conversion Rate

Supporting KPIs:

* Landing Page Visit Rate
* Trial Start Rate
* Onboarding Completion Rate
* Average Revenue Per User
* Average Revenue Per Converted User
* Engagement Score

Guardrail Metrics:

* Refund Rate
* Support Ticket Rate
* Average Days to Convert

Segment Analysis:

* Region
* Device Type
* Traffic Source

---

# Experiment Analysis Approach

The experiment compared users in the Control and Treatment groups.

The analysis included:

1. Calculating key business metrics for both groups.
2. Comparing conversion funnel performance.
3. Measuring revenue-related metrics.
4. Evaluating guardrail metrics to identify potential risks.
5. Performing segment-level analysis by Region, Device Type, and Traffic Source.
6. Conducting a statistical hypothesis test to determine whether the observed improvement in paid conversion was statistically significant.

---

# Hypothesis Test Summary

Primary Metric:
Paid Conversion Rate

Statistical Test:
One-tailed Two-Proportion Z-Test

Hypotheses:

* Null Hypothesis (H₀): The treatment does not improve the paid conversion rate.
* Alternative Hypothesis (H₁): The treatment improves the paid conversion rate.

Results:

* Control Conversion Rate: **3.17%**
* Treatment Conversion Rate: **6.99%**
* Z-statistic: **3.252**
* P-value: **0.000573**

Since the p-value is less than the significance level of 0.05, the null hypothesis is rejected. The treatment produced a statistically significant improvement in paid conversion.

---

# Guardrail Metrics Considered

To ensure that the increase in conversion did not negatively impact the business, the following guardrail metrics were evaluated:

* Refund Rate
* Support Ticket Rate
* Average Engagement Score
* Average Days to Convert

Key Findings:

* Refund rate increased slightly but remained very low.
* Support ticket rate increased, indicating a need for continued monitoring.
* Engagement score improved.
* Users converted faster under the treatment.

Overall, no guardrail metric indicated a significant business risk.

---

# Final Recommendation

**Recommendation: Launch**

The treatment achieved a statistically significant improvement in paid conversion while maintaining acceptable performance across key guardrail metrics.

Although support ticket rates increased slightly, improvements in conversion rate, engagement, and conversion speed outweigh the associated risks.

The treatment should be launched while continuing to monitor customer support demand and refund behaviour after deployment.

---

# Assumptions and Limitations

## Assumptions

* Users were randomly assigned to the Control and Treatment groups.
* The experiment duration was sufficient to capture user behaviour.
* The dataset accurately reflects user actions.
* Revenue and conversion data are complete and reliable.

## Limitations

* The experiment represents a limited time period.
* Long-term customer retention was not evaluated.
* Refund behaviour may change over time.
* External factors affecting user behaviour were not included.
* Results may differ across future user populations.


