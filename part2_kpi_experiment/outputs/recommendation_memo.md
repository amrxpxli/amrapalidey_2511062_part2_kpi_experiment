# Task 1: Business Problem Summary:

The objective of this experiment is to determine whether the new onboarding campaign should replace the existing onboarding process. The decision affects company leadership, product, marketing, and customer success teams, as well as future users. Success is measured primarily by an improvement in the paid conversion rate while ensuring that guardrail metrics such as refund rate, support ticket rate, engagement score, and days to convert remain within acceptable limits. The recommendation will be based on statistical evidence from hypothesis testing, guardrail analysis, and segment-level performance.

# Task 8: Guardrail Metrics Evaluation

## Objective

Although the treatment significantly improved the primary metric (paid conversion rate), it is important to verify that the improvement does not negatively affect other important business metrics.

### Guardrail Metric 1: Refund Rate

| Group     | Refund Rate |
| --------- | ----------: |
| Control   |       0.00% |
| Treatment |       0.42% |

**Interpretation:**
The treatment group recorded a very small refund rate (0.42%), whereas the control group had no refunds. While this is a slight increase, the rate is extremely low and does not currently represent a major business risk. However, it should continue to be monitored after rollout.

---

### Guardrail Metric 2: Support Ticket Rate

| Group     | Average Support Tickets |
| --------- | ----------------------: |
| Control   |                   0.219 |
| Treatment |                   0.372 |

**Interpretation:**
Users in the treatment group generated more support tickets than those in the control group. This may indicate that some users experienced confusion or required additional assistance with the new onboarding experience. Although the increase is noticeable, it is relatively small compared with the improvement in conversion.

---

### Guardrail Metric 3: Days to Convert

| Group     | Average Days to Convert |
| --------- | ----------------------: |
| Control   |               8.86 days |
| Treatment |               6.40 days |

**Interpretation:**
The treatment helped users convert approximately 2.5 days faster than the control group. Faster conversion is a positive outcome because it improves cash flow and reduces the risk of losing users before subscription.

---

### Guardrail Metric 4: Engagement Score

| Group     | Average Engagement Score |
| --------- | -----------------------: |
| Control   |                    57.03 |
| Treatment |                    62.93 |

**Interpretation:**
Users exposed to the new onboarding campaign showed higher engagement, suggesting that the treatment not only increased conversions but also encouraged greater product usage.

---

## Overall Guardrail Assessment

The treatment shows one minor risk—a slight increase in support tickets and a very small refund rate. However, these are outweighed by substantial improvements in conversion rate, engagement, and faster conversion time. Overall, no guardrail metric presents a significant risk that would prevent rollout.

# Task 9
## Recommendation Memo

## Executive Summary

The A/B experiment evaluated a new onboarding campaign designed to improve paid subscription conversion. Statistical analysis shows that the treatment significantly increased the conversion rate from 3.17% to 6.99% (p-value = 0.000573). Guardrail metrics indicate higher engagement and faster conversion, with only a small increase in support tickets and refunds. Overall, the treatment demonstrates a positive business impact.

---

## North Star Metric

Paid Conversion Rate (Converted to Paid Subscription)

---

## KPI Tree Explanation

**Business Goal:** Increase subscription revenue

* North Star Metric

  * Paid Conversion Rate
* Supporting KPIs

  * Trial Started
  * Onboarding Completion
  * Engagement Score
  * Revenue in First 30 Days
* Guardrail Metrics

  * Refund Rate
  * Support Ticket Rate
  * Days to Convert

---

## Experiment Result Summary

* Control Users: 693
* Treatment Users: 715
* Control Conversion Rate: 3.17%
* Treatment Conversion Rate: 6.99%

The treatment improved the conversion rate by approximately 3.8 percentage points, representing more than a two-fold increase.

---

## Hypothesis Test Interpretation

A one-tailed two-proportion Z-test was performed.

* Z-statistic: 3.252
* P-value: 0.000573

Since the p-value is less than the significance level of 0.05, the null hypothesis is rejected. The new onboarding campaign produced a statistically significant improvement in paid conversion.

---

## Guardrail Analysis

* Refund rate increased slightly (0.42%) but remains very low.
* Support tickets increased from 0.219 to 0.372 per user, suggesting additional user assistance may be required.
* Average days to convert decreased from 8.86 to 6.40 days.
* Average engagement score increased from 57.03 to 62.93.

Overall, the positive outcomes outweigh the minor risks.

---

## Segment-Level Insight

The treatment improved conversion across all regions.

| Region | Control | Treatment |
| ------ | ------: | --------: |
| North  |   3.45% |     8.89% |
| South  |   3.26% |     7.61% |
| East   |   2.53% |     6.40% |
| West   |   3.38% |     5.03% |

The North region showed the strongest improvement, while the West region showed the smallest gain. No segment experienced a decline.

---

## Final Recommendation

**Recommendation: Launch**

The treatment delivers a statistically significant improvement in the primary business objective while maintaining acceptable guardrail metrics. Although support tickets increased slightly, improvements in conversion, engagement, and faster activation outweigh this risk.

---

## Risks and Limitations

* The experiment covers only the available sample and observation period.
* Refunds may increase over a longer time horizon.
* Increased support requests should be monitored after rollout.
* Results may differ for future customer populations.

---

## Next Steps

1. Roll out the new onboarding campaign to all users.
2. Monitor support ticket volume and refund rate during the rollout.
3. Continue tracking engagement and revenue after deployment.
4. Perform follow-up analyses by device type, traffic source, and subscription plan to identify additional optimization opportunities.
