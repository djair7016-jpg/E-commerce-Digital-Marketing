# E-commerce Marketing and A/B Test Analysis

## Executive Summary

An e-commerce company wanted to determine whether a new landing-page experience could improve customer conversion and support better marketing decisions.

I analyzed an A/B experiment using Python, comparing conversion performance between the control and treatment variants. I also examined differences across acquisition channels and customer types to understand whether the results were consistent among user segments.

Variant B achieved a conversion rate of 15.96%, compared with 12.57% for Variant A, representing an improvement of 3.39 percentage points. The difference was statistically significant (`p = 0.016`), providing evidence that the new experience generated better conversion results.

Based on the experiment, I recommended deploying Variant B while continuing to monitor its performance across acquisition channels and customer segments.

## Business Problem

The project addressed four business questions:

- Did the new landing-page variant improve conversion?
- Was the observed difference statistically significant?
- Which acquisition channels generated the strongest conversion rates?
- Did new and returning customers respond differently to the experience?

The objective was to move beyond descriptive metrics and use statistical evidence to support a product and marketing decision.

## Dataset and Scope

The dataset included information about:

- Experiment variant
- Conversion outcome
- Acquisition channel
- Customer type
- User-level behavior
- Marketing-related variables

The analysis focused on comparing conversion performance between the control and treatment groups while also examining relevant customer segments.

## Analytical Approach

### 1. Data Preparation

I used Python and Pandas to:

- inspect data types and missing values;
- verify experiment-group consistency;
- review duplicates and invalid observations;
- prepare categorical variables for analysis;
- calculate conversion metrics by variant and segment.

### 2. Conversion Analysis

I calculated conversion rates for both experiment groups:

- Variant A: 12.57%
- Variant B: 15.96%
- Difference: 3.39 percentage points

### 3. Statistical Testing

I applied a statistical hypothesis test to determine whether the difference between variants could reasonably be attributed to chance.

The resulting p-value was `0.016`, below the 0.05 significance threshold. Therefore, the null hypothesis of equal conversion performance was rejected.

### 4. Segment Analysis

Conversion was also evaluated by:

- acquisition channel;
- new versus returning customers;
- experiment variant.

This helped determine whether the overall result remained relevant across different user groups.

## Key Findings

- Variant B achieved a higher conversion rate than Variant A.
- The difference of 3.39 percentage points was statistically significant.
- Referral generated a conversion rate of approximately 13.88%, slightly above Organic at 13.79%.
- New customers converted at approximately 14.36%, compared with 14.09% for returning customers.
- Segment differences were relatively small compared with the effect observed between experiment variants.

## Business Recommendations

- Deploy Variant B as the primary landing-page experience.
- Monitor conversion after deployment to confirm that the experimental uplift is sustained.
- Analyze conversion by acquisition channel before reallocating marketing investment.
- Continue testing landing-page elements such as messaging, calls to action, and checkout progression.
- Avoid assuming that statistically significant conversion automatically guarantees higher long-term profitability; revenue and customer value should also be monitored.

## Tools and Techniques

- Python
- Pandas
- NumPy
- SciPy
- Matplotlib
- Seaborn
- A/B testing
- Hypothesis testing
- Conversion analysis
- Customer segmentation

## Visualizations

### Conversion by Variant

![Conversion by Variant](images/conversion_by_variant.png)

### Conversion by Acquisition Channel

![Conversion by Channel](images/conversion_by_channel.png)

### Conversion by Customer Type

![Conversion by Customer Type](images/conversion_by_customer_type.png)

## Repository Structure

```text
notebooks/  Data preparation, analysis, and statistical testing
images/     Main visualizations and results
README.md   Project documentation
