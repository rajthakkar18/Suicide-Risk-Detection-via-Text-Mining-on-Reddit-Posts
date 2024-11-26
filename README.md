# Suicide-Risk-Detection-via-Text-Mining-on-Reddit-Posts (SAS)

**Overview**
This project leverages text mining techniques to analyze Reddit posts and identify risks of suicidality. Using machine learning models, we classify posts into categories based on their potential indicators of self-harm or suicide. This analysis can aid in early detection and intervention, potentially saving lives.

**Dataset**
Source: Anonymized Reddit posts dataset.
Size: 500 posts.
Categories:
Supportive
Attempt
Ideation
Indicator
Behavior
Posts are labeled based on suicidality risk, with merged categories to address data imbalance:
Attempt + Behavior → Attempt
Ideation + Indicator → Ideation

**Objectives**
1. Analyze patterns in suicidality-related posts.
2. Build predictive models to classify posts into risk categories.
3. Explore the potential of text mining for mental health analytics.

****Methodology****
**Preprocessing**
1. Data Cleaning: Addressed inconsistencies in merged text and labels.
2. Category Balancing: Combined underrepresented categories.
3. Text Filtering: Adjusted term frequency thresholds and applied customized stop lists.
4. Clustering: Grouped posts using Singular Value Decomposition (SVD).

**Models and Techniques**
Models:
1. Decision Tree
2. Logistic Regression
3. Memory-Based Reasoning (MBR)

Term Weighting:
1. Entropy
2. Inverse Document Frequency (IDF)
3. Mutual Information

Best-performing model: Decision Tree with Entropy (64% accuracy, 36% misclassification rate).

**Challenges**
Limited dataset size causing imbalances and low representation of critical categories.
High sensitivity of language context, leading to some misclassifications.

**Results**
The Decision Tree model using Entropy outperformed others, effectively distinguishing risk levels.
Highlights the importance of refined text preprocessing and feature engineering.

**Future Work**
Expand Dataset: Incorporate more posts for better model training.
Multi-word Terms: Improve context understanding using phrases like “end my life.”
Enhanced Stop Lists: Tailor stop lists to the domain for better noise reduction.

**Conclusion**
This project demonstrates the potential of text mining for suicide prevention. With further development, the approach can support mental health professionals by identifying individuals at risk earlier and more effectively.


