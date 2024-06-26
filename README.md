## Future Availability:
We plan to make the code and data publicly available upon acceptance of the manuscript. 
## CrisisSpot

We propose a novel framework, **CrisisSpot**, designed to effectively identify crisis-related information. It consists of four integral components:

1. **Feature Extraction and Interaction Module:** Orchestrates interaction between text and visual modalities via an IDEA attention mechanism.

2. **Multimodal Graph Learning:** Enriches features extracted from a multimodal encoder and then reconstructed enriched features through a GraphSAGE layer.

3. **Social Context Feature Extraction:** Extracts diverse attributes such as crisis-related information and user interaction history, quantified by metrics like User Informative Score (UIS), Crisis Informative Score (CIS), and User Engagement.

4. **Multimodal Fusion Module:** Processes fused features from the previous modules, integrating them via a Joint Fusion Learning Network for effective crisis-related information discernment.



# TSEqD: Turkey-Syria Earthquake Dataset
The TSEqD multimodal Twitter dataset is a comprehensive collection of manually annotated comprising 10,352 tweets and associated images obtained during the period from February 6, 2023, to March 16, 2023. TSEqD is annotated for two distinct tasks: Informative Tasks and Humanitarian Tasks. The process of data curation, annotation, and label distribution across various classes is elaborated in subsequent sections, ensuring a comprehensive understanding of the dataset's composition and utility.

## Task 1: Informative vs Not informative
Task 1 involves identifying and categorizing informative content within the TSEqD Dataset. Informative content refers to social media posts that convey meaningful information related to the Turkey-Syria Earthquake. The goal of Task 1 is to label each sample as either informative or non-informative based on the presence or absence of valuable information regarding the earthquake event. This task is crucial for enabling efficient information retrieval, aiding disaster response efforts, and facilitating research on public communication during natural disasters.
| Description        | Label | Text | Image |
|--------------------|-------|------|-------|
| Informative        | 1     | 7136 | 5363  |
| Non-Informative    | 0     | 3199 | 4972  |


## Task 2: Humanitarian Categories
Task 2 focuses on identifying and categorizing specific humanitarian aspects within the TSEqD Dataset. This task involves classifying social media posts into different humanitarian categories, such as infrastructure and utility damage, vehicle damage, rescue and donation efforts, reports of injured or deceased individuals, affected individuals, missing or found people, other relevant information, and posts that are not relevant or cannot be judged in the context of humanitarian aid and disaster response. The objective of Task 2 is to provide granular insights into the types of humanitarian needs and responses documented within the dataset, facilitating targeted assistance and resource allocation in disaster-affected areas.
| Description                       | Label | Text | Image |
|-----------------------------------|-------|------|-------|
| Infrastructure and Utility Damage | 1     | 131  | 1279  |
| Vehicle Damage                    | 2     | 0    | 46    |
| Rescue and Donation               | 3     | 4235 | 1659  |
| Injured or Dead People           | 4     | 1182 | 199   |
| Affected Individuals             | 5     | 492  | 1125  |
| Missing or Found People          | 6     | 83   | 12    |
| Other Relevant Information        | 7     | 1015 | 1041  |
| Not Relevant or Can’t Judge      | 8     | 3197 | 4974  |

### Distribution of Labels in the TSEqD Dataset
Given the complex nature of multimodal posts, where labels for text and images may differ, it's essential to discern and account for such variations. We present the distribution of these instances in the following table, shedding light on the diverse annotations across modalities.
| Label                    | Count |
|--------------------------|-------|
| Both Informative         | 4312  |
| At least one Informative | 8187  |
| Non-Informative          | 2148 

