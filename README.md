
# CrisisSpot

We propose a novel framework, **CrisisSpot**, designed to effectively identify crisis-related information. It consists of four integral components:

1. **Feature Extraction and Interaction Module** orchestrates the interaction between text and visual modalities via an IDEA attention mechanism.

2. **Multimodal Graph Learning Module** enriches features extracted from a multimodal encoder and then reconstructs enriched features through a GraphSAGE layer.

3. **Social Context Feature Extraction** extracts diverse attributes such as crisis-related information and user interaction history, quantified by metrics such as User Informative Score (UIS), Crisis Informative Score (CIS), and User Engagement History.

4. **Multimodal Fusion Module** processes fused features from the previous modules, integrating them via a Joint Fusion Learning Network for effective crisis-related information classification.

### CrisisSpot Architecture

Below is the architecture of the **CrisisSpot** framework:

<p align="center">
  <img src="https://raw.githubusercontent.com/Shahid-135/CrisisSpot/main/final_arch.png" alt="CrisisSpot Architecture"/>
  <br>
  <em>Figure 1: Overview of the CrisisSpot architecture.</em>
</p>


# TSEqD: Turkey-Syria Earthquake Dataset
The TSEqD multimodal dataset is a comprehensive collection of manually annotated comprising 10,352 tweets and associated images obtained during the period from February 6, 2023, to March 16, 2023. TSEqD is annotated for two distinct tasks: Informative Tasks and Humanitarian Tasks. The process of data curation, annotation, and label distribution across various classes is elaborated in subsequent sections, ensuring a comprehensive understanding of the dataset's composition and utility.

## Task 1: Informative vs Not informative
Task 1 involves identifying and categorizing informative and non-informative content within the TSEqD Dataset. Informative content refers to social media posts that convey meaningful information related to the Turkey-Syria Earthquake. The goal of Task 1 is to label each sample as either informative or non-informative based on the presence or absence of valuable information regarding the earthquake event. This task is crucial for enabling efficient information retrieval, aiding disaster response efforts, and facilitating research on public communication during natural disasters.
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

# Dataset Access
**Access to the dataset is restricted to academic and research purposes. To request access, please ensure compliance with the following requirements:**

- **Non-Commercial Use**: The dataset is provided exclusively for academic research and non-commercial purposes. Any form of commercial use, direct or indirect, is strictly prohibited. It must not be used to develop or market commercial products or services.

- **No Redistribution**: The dataset must not be redistributed, republished, or shared in any form, whether in full or in part, across any public or private repositories, platforms, or social media. Users must store the dataset in secure environments and ensure that unauthorized parties do not gain access.

- **Compliance with Platform Policies**: As this dataset is derived from publicly available Twitter (now X) data, users must comply with the platform's Developer Agreement and Policies. This includes adhering to data usage and privacy guidelines, ensuring that no actions breach content redistribution rules.

- **Academic Integrity**: The dataset must only be used for legitimate academic research. Researchers are responsible for ensuring that their use of the dataset does not contravene any ethical standards, particularly regarding data privacy and responsible usage.

1. **Important:** Use your **institutional email address** when submitting the form. Requests from personal email addresses will not be considered.
2. First, please fill out this [Consent Form](https://docs.google.com/document/d/1xqshqL6nlss246QZSY6TE0kWtAbhRbxK/edit?usp=sharing&ouid=117095985932126675899&rtpof=true&sd=true), and then upload it in the [Dataset Request Form]( https://docs.google.com/forms/d/e/1FAIpQLSdklbRkvXfqMp9tKQj-Ue1oFy-XKVIkv_DqARgyjwWLJxracg/viewform?embedded=true) along with your details.

Once your request is reviewed and approved, you will receive an email with instructions on how to download the dataset.

## Precomputed Embeddings

We are providing the precomputed embeddings for this dataset, which can be directly utilized for various downstream tasks. These embeddings are optimized for performance and can help accelerate your research by enabling quick experimentation without the need for extensive preprocessing. You can access the embeddings [here](https://drive.google.com/drive/folders/17gQ1_UoXwJPvdNBRhL7PGBwpRwhzGx9s?usp=sharing).


<!DOCTYPE html>
<html lang="en">
<body>
<h1>Citation</h1>
<p>If you find this work useful or use the dataset in your research, please cite it as follows:</p>
<pre>
<code id="citation">
@article{DAR2025125337,
  title = {A social context-aware graph-based multimodal attentive learning framework for disaster content classification during emergencies},
  journal = {Expert Systems with Applications},
  volume = {259},
  pages = {125337},
  year = {2025},
  issn = {0957-4174},
  doi = {https://doi.org/10.1016/j.eswa.2024.125337},
  url = {https://www.sciencedirect.com/science/article/pii/S0957417424022048},
  author = {Shahid Shafi Dar and Mohammad Zia Ur Rehman and Karan Bais and Mohammed Abdul Haseeb and Nagendra Kumar}
}
</code>
</pre>

<button onclick="copyToClipboard()"></button>
</body>
</html>
