# Mobile Phone Data Tutorial

## Tutorial Description

This hands-on tutorial guides participants through the complex reality of working with Call Detail Records (CDR) data, using a real 3-month dataset from Chile as our primary case study. Rather than presenting an idealized scenario, we focus on common data quality issues, biases, and methodological challenges that analysts typically encounter. Participants will learn practical strategies for handling missing data, addressing sampling biases, and extracting meaningful mobility patterns despite data limitations.
## Dataset Overview

- **3 months of CDR data**, for more technical information on this dataset, you can consult [this paper](https://www.nature.com/articles/s41599-020-0500-x). 
- **Some demographic attributes for customers**:
  - Gender
  - Number of lines owned (important if we'd like to make sure the demographic info is more correct)
  - Nationality (Chilean/non-Chilean)
  - Socio-economic group
- Known challenges:
  - Missing tower information
  - Hub tower effects
  - Incomplete caller/callee information
  - Sampling biases from single-operator data
  - **IMPORTANTLY: this is just one dataset**. How representative it is compared to similar datasets (or with other countries), I don't know. We've made some progress in validating the results with other datasets, particularly [Meta's](https://arxiv.org/abs/2410.06017) and [Google and Apple mobility](https://web.archive.org/web/20210520152647/https://leoferres.info/blog/2020/08/03/im1-vs-google-vs-apple-mobility/), but, except for the first, the other two are not formally published. I'm kind of convinced with the analyses, though.
## Detailed Schedule (3 hours)

**1. Introduction: Understanding Your Data (25 minutes)**

- CDR data structure and limitations
- Walking through our Chilean dataset
- Common pitfalls in CDR analysis
- Initial data assessment techniques
- _Exercise:_ Basic exploratory analysis to identify data quality issues

**2. Data Quality and Preprocessing (40 minutes)**

- Handling missing tower information
- Identifying and managing hub towers
- Dealing with incomplete demographic information
- Addressing temporal gaps
- _Practical Exercise:_ Developing cleaning procedures for problematic towers and incomplete records

**3. Individual Mobility Metrics (35 minutes)**

- Computing robust metrics despite data limitations:
    - Radius of gyration with missing locations
    - Activity space analysis
    - Location entropy and predictability
    - Most frequent locations detection
    - Jump lengths and waiting times
- Handling temporal sparsity in individual trajectories
- _Practical Exercise:_ Calculating and validating individual mobility metrics

**4. Break (15 minutes)**

**5. Collective Mobility Patterns (35 minutes)**

- Trajectory analysis techniques:
    - Origin-Destination matrices with incomplete data
    - Flow analysis and visualization
    - Temporal patterns of collective movement
    - Impact of hub towers on trajectory analysis
- Aggregation strategies for robust analysis
- _Practical Exercise:_ Building and visualizing collective mobility flows

**6. Socio-demographic Analysis (20 minutes)**

- Combining mobility metrics with demographic attributes
- Analyzing mobility patterns by:
    - Gender differences in mobility
    - Socio-economic group variations
    - Chilean vs non-Chilean mobility patterns
- Understanding and addressing selection bias
- _Exercise:_ Comparative analysis of mobility metrics across groups

**7. Validation and Interpretation (10 minutes)**

- Cross-validation with external data sources
- Understanding the limits of inference
- Communicating uncertainties
- Ethics and privacy considerations

