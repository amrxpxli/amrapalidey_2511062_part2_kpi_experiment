# Task 6 : Hypothesis Test Notes 

## Business Context

The company introduced a new onboarding and activation campaign (Treatment) to improve user activation, engagement, and subscription conversion. Users were randomly assigned to either the existing onboarding experience (Control) or the new onboarding experience (Treatment).

The primary business objective is to determine whether the Treatment campaign leads to a statistically significant improvement in business performance and should therefore be rolled out to all users.

---

# Metric Being Tested

**Primary Metric:** Paid Conversion Rate

Paid Conversion Rate is defined as:

> Number of users who converted to a paid subscription ÷ Total number of users

This metric is the primary Key Performance Indicator (KPI) because it directly measures whether the onboarding campaign generates more paying customers, which is the main objective of the business.

---

# Null Hypothesis (H₀)

There is **no statistically significant difference** in the Paid Conversion Rate between the Control group and the Treatment group.

Mathematically,

**H₀:**

[
p_{Treatment} = p_{Control}
]

or equivalently,

[
p_{Treatment} - p_{Control} = 0
]

where:

* (p_{Treatment}) = Paid Conversion Rate of the Treatment group
* (p_{Control}) = Paid Conversion Rate of the Control group

---

# Alternative Hypothesis (H₁)

The Treatment group has a **higher Paid Conversion Rate** than the Control group.

Mathematically,

**H₁:**

[
p_{Treatment} > p_{Control}
]

This hypothesis reflects the company's expectation that the new onboarding experience increases customer conversion.

---

# Type of Test

**One-tailed hypothesis test**

### Reason

The company is only interested in determining whether the Treatment performs **better** than the Control.

If the Treatment performs worse, it will simply not be deployed.

Therefore, a one-tailed test is appropriate because only improvement is of business interest.

---

# Significance Level

[
\alpha = 0.05
]

A 5% significance level means there is a maximum acceptable probability of 5% of incorrectly concluding that the new onboarding campaign is better when it is actually not (Type I Error).

This is the standard significance level used in A/B testing and business experimentation.

---

# Reason for Choosing Paid Conversion Rate

Paid Conversion Rate was selected because:

* It directly measures business growth.
* It reflects the success of the onboarding campaign in converting users into paying customers.
* It has a direct impact on subscription revenue.
* Leadership ultimately decides on rollout based on whether more users become paying subscribers.

Although onboarding completion and engagement are valuable supporting metrics, they only create business value if they ultimately increase paid conversions.

---

# Interpretation Logic

After performing the statistical hypothesis test:

### If p-value < 0.05

* Reject the Null Hypothesis.
* Conclude that the Treatment significantly improves Paid Conversion Rate.
* If guardrail metrics (Refund Rate and Support Ticket Rate) remain acceptable, recommend rolling out the new onboarding campaign to all users.

---

### If p-value ≥ 0.05

* Fail to reject the Null Hypothesis.
* Conclude that there is insufficient statistical evidence that the Treatment improves Paid Conversion Rate.
* Recommend keeping the existing onboarding experience or conducting further experimentation before rollout.

---

# Business Decision

The final rollout decision should consider both:

## Primary Success Metric

* Paid Conversion Rate

## Guardrail Metrics

* Refund Rate
* Support Ticket Rate
* Average Days to Convert

A rollout is recommended only if the Treatment produces a statistically significant increase in Paid Conversion Rate **without negatively affecting the guardrail metrics**.

This ensures that business growth is achieved without reducing customer satisfaction or increasing operational costs.



# Hypothesis Test Analysis

## Business Objective

The objective of this analysis is to determine whether the new onboarding campaign (Treatment) significantly improves the Paid Conversion Rate compared to the existing onboarding experience (Control).

The result of this hypothesis test will help leadership decide whether the Treatment should be rolled out to all users.

---

# Test Performed

**Test Name**

Two-Proportion Z-Test

---

# Primary Metric

Paid Conversion Rate

Definition:

Number of users who converted to a paid subscription divided by the total number of users in each experiment group.

---

# Test Inputs

| Parameter          | Value                   |
| ------------------ | ----------------------- |
| Control Group      | Existing onboarding     |
| Treatment Group    | New onboarding campaign |
| Metric Tested      | Paid Conversion Rate    |
| Outcome Variable   | converted_to_paid       |
| Significance Level | 0.05                    |
| Test Type          | One-tailed              |

---

# Hypotheses

### Null Hypothesis (H₀)

The Paid Conversion Rate of the Treatment group is equal to that of the Control group.

[
p_{Treatment}=p_{Control}
]

---

### Alternative Hypothesis (H₁)

The Treatment group has a higher Paid Conversion Rate than the Control group.

[
p_{Treatment}>p_{Control}
]

---

# Test Output

The Two-Proportion Z-Test was performed to compare the Paid Conversion Rates of the two groups.

The statistical output includes:

* Control Conversion Rate
* Treatment Conversion Rate
* Z Statistic
* P-value

(See **screenshots/hypothesis_test_output.png**)

---

# Decision Rule

If

```
P-value < 0.05
```

Reject the Null Hypothesis.

Otherwise,

Fail to Reject the Null Hypothesis.

---

# Business Interpretation

### If p-value < 0.05

The Treatment onboarding campaign significantly improves the Paid Conversion Rate.

Provided that guardrail metrics (Refund Rate and Support Ticket Rate) remain acceptable, the Treatment should be recommended for rollout to all users.

---

### If p-value ≥ 0.05

There is insufficient statistical evidence that the Treatment improves Paid Conversion Rate.

The company should continue with the existing onboarding experience or conduct additional experiments before making a rollout decision.

---

# Conclusion

The hypothesis test provides statistical evidence supporting the business decision regarding whether the new onboarding campaign should replace the existing onboarding experience.
