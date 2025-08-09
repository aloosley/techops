Documentation Template for Compliance with the EU AI Act
### AI system General information
- AI System Name:
    
- Version Number:
    
- Date of Documentation:
    
- Organization / Provider / Deployer:
    
- Release Date:
    
- Last Update:
    
- Contact Information:
    
- System Description:  
    A brief overview of the AI system, its purpose, the context of use, and key functionalities.

### Intended Purpose
**Description of the Intended Use:** Detail what the AI system is designed to do, including its main functionalities and objectives.

**Target Users:** Identify the specific groups or industries that the AI system is intended for, such as healthcare professionals, financial analysts, or general consumers.

**Operational Environment:** Describe where and how the AI system will operate, such as on mobile devices, cloud platforms, or embedded systems.

**Geographical Scope:** Specify the countries or regions where the AI system will be deployed and used.
 


 #### Suitable Use Case(s)
<!-- scope: periscope -->
<!-- info: Summarize known suitable and intended use cases of this dataset.

Use additional notes to capture any specific patterns that readers should
look out for, or other relevant information or considerations. -->
**Suitable Use Case:** Summarize here. Include links where necessary.

**Suitable Use Case:** Summarize here. Include links where necessary.

**Suitable Use Case:** Summarize here. Include links where necessary.

**Additional Notes:** Add here

#### Unsuitable Use Case(s)
<!-- scope: microscope -->
<!-- info: Summarize known unsuitable and unintended use cases of this dataset.

Use additional notes to capture any specific patterns that readers should look
out for, or other relevant information or considerations. -->
**Unsuitable Use Case:** Summarize here. Include links where necessary.

**Unsuitable Use Case:** Summarize here. Include links where necessary.

**Unsuitable Use Case:** Summarize here. Include links where necessary.



### Technical Specifications and System Architecture

**Architecture Description:** Provide a high-level diagram or description of the AI system’s architecture, highlighting the main components and data flow.

**Components and Modules:** List and describe each component or module, including software libraries, APIs, and hardware elements involved.

**Model Selection:**

**AI Model selected:**
 Specify the types of algorithms and models used, such as supervised learning models, reinforcement learning agents, convolutional neural networks.

**Training Methodologies:** Explain how the AI models were trained, including data preprocessing steps, training procedures, and validation techniques.
==Patrick says: data preprocessing should be a separate part. Data preprocessing is not just a part of training, also of inference.  It is in fact already included in the "data pre-processing" below.  Probably just removing it here should suffice.==

**Hardware and Software Requirements:** Outline the minimum hardware specifications and software dependencies required to run the AI system.



#### Relevant Links
<!-- info: Provide a list of relevant links for quick accessibility
by documentation consumers.

The examples below represent
: -->
<!-- width: full -->
* [Dataset Link] - i.e. link to S3 bucket, SQL or Big Query tables, etc.
* [Initiative Link] - i.e. link to initiative through which the curation of this dataset was carried out
* [Code Repository Links] - i.e. link to GitHub, GitLab or other type of code repository
* [Data Quality Monitoring Link(s)] - i.e. link to Data Quality Framework dashboard
* [Labeling Job Link(s)] - i.e. link to SageMaker Ground Truth job
* [Governance Processes Lin(s)] - i.e. link to review process for obtaining permission to access dataset for use on a specific use case

### Data Governance Documentation
**Dataset Name:**
**Creator/Curator:**
**Version:**
**Source:**
**License:**
**Date Created:**
**Last Updated:**
**Link to Dataset (if available):** i.e. link to S3 bucket, SQL or Big Query tables, etc.


#### Dataset Status
<!-- scope: telescope -->
<!-- info: Select **one:** -->
**Status Date:** DD/MM/YYYY

**Under Preparation** - The dataset is still under active curation and is not yet ready for use due to active "dev" updates.

**Regularly Updated** - New versions of the dataset have been or will continue to be made available.

**Actively Maintained** - No new versions will be made available, but this dataset will be actively maintained, including but not limited to updates to the data.

**Limited Maintenance** - The data will not be updated, but any technical issues will be addressed.

**Deprecated** - This dataset is obsolete or is no longer being maintained.

#### Dataset Characteristics
**Data Types:** (e.g., images, text, audio, structured, unstructured data)
**Size/Volume:**
**Number of Instances/Records:**
**Primary Use Case(s):** Description of the main AI use cases that the dataset was designed for or is typically used in.
**Associated AI System(s):** List the AI system(s) that this dataset is or has been used in.
**Number of Features/Attributes:**
**Label Information (if applicable):**
**Operational environment:** Describe where and how the AI system will operate, such as on mobile devices, cloud platforms, or embedded systems.
**Geographical Scope:** Geographic location(s) where the data was collected.
**Date of Collection:** Start and end date of data collection.
#### Data Origin and Source
**Source(s):** Provide information about where the data was sourced from (e.g., sensors, surveys, web scraping, public databases).
**Third-Party Data:** Indicate if any part of the dataset was obtained from third parties, and if so, detail the legal agreements in place (license, usage rights, etc.).
**Ethical Sourcing:** (Ghana issues) Provide information on the ethical and legal compliance of the data collection process (e.g., informed consent, transparency to data subjects, and compliance with GDPR or other regulations).
    
#### Data Pre-Processing
**Data Collection**
- Source(s) of the data:
- File format(s) and storage location(s):
    

**Data Cleaning**
- Handling missing data: (e.g., removal, imputation method used)
- Outlier treatment: (e.g., detection and removal technique)
- Duplicates removal: (Yes/No)
- Error correction: (Manual/Automated, if applicable)
    

**Data Transformation**

- Normalization/Standardization: (Method used, e.g., min-max scaling)
    
- Encoding categorical data: (e.g., one-hot encoding, label encoding)
    
- Text/tokenization: (Applicable for NLP tasks)
    

**Feature Engineering**

- Feature selection: (e.g., methods used to select features)
    
- Feature extraction: (e.g., PCA, interaction terms)
    
- Newly created features: (List any)
    

**Data Splitting**

- Train-test split ratio: (e.g., 80/20, 70/30) ==Patrick says: this should be part of the training, not of the data processing.  Remove here.==
    
- Cross-validation: (If used, mention k-fold, etc.) ==Patrick says: this should be part of the training, not of the data processing.  And anyway half-duplicate of the above.  Remove here.==
    

**Dimensionality Reduction (Optional)**

- Technique(s) used: (e.g., PCA, t-SNE)
    
- Number of dimensions after reduction: (Specify)
    

**Data Augmentation** (Optional, for images/text)

- Augmentation technique(s): (e.g., rotation, flipping for images)
    

**Data Shuffling**

- Shuffle applied: (Yes/No)  ==Patrick says: this should be part of the training, not of the data processing. Remove here.==
    
#### Data Annotation and Labeling (this could be part of Human Oversight)

- Annotation Process: Describe the process used to label or annotate the data (e.g., human labelers, automated, crowdsourcing).
    
- Quality Assurance: Explain any quality control mechanisms applied to ensure accurate labeling or annotation.
    
- Inter-Annotator Agreement: If applicable, mention how disagreements in labeling were resolved.
    
#### 3.8 Dataset Distribution and Licensing

- Availability:
    
- Open/public or private dataset
    
- Commercial restrictions ==instead of this and the last point of this section, it suffices to add the license==
    

- Dataset Documentation Link: (Link to further details if available)
    
- User Rights and Limitations:


#### 3.9 Data Versioning
**Data Version Control Tools :**
    
- DVC (Data Version Control): Tracks datasets, connects them to model versions, and integrates with Git.
    
- Git-LFS (Large File Storage): Stores large data files outside the Git repository.
    
- Delta Lake: Tracks changes in structured data (e.g., data lakes).
    
- Pachyderm: Offers data pipelines with built-in versioning.

### Maintain Metadata and Schema Versioning
    
 Why: Data formats, schema, and other metadata changes can impact downstream processes. Tracking these ensures transparency.

#### How:

Create a data dictionary:
    

- Document dataset structure, column descriptions, data types, and relationships.
    

Track schema changes:
    

- Use tools like dbt or Great Expectations to log schema evolution.
    
- Record changes as part of version control or data pipelines.
    

 Save metadata alongside datasets:
    

- Use JSON, YAML, or similar formats to store metadata files.
    
- Include details like source, timestamp, description, version, and quality metrics.
    
  

 #### Incorporate Data Lineage Tools
    
 Why: Data lineage tools provide end-to-end visibility of data transformations and dependencies.

#### How:

- Integrate tools like OpenLineage, Talend, or Alation.
    
- Track data movement: From ingestion to transformation to storage.
    
-  Visualise: Lineage graphs showing how different dataset versions relate.

#### Known Usages
<!-- info: Fill out the following section if the dataset has any
current known usages.
-->
#### Model(s)
<!-- scope: telescope -->
<!-- info: Provide a table of known models
that use this dataset.
-->

| **Model**           | **Model Task**       | **Purpose of Dataset Usage** |
|---------------------|----------------------|------------------------------|
| [Example Model 1]() | Image Segmentation   | Fairness evaluation          |
| [Example Model 2]() | Skin Tone Classifier | Training and validation      |

Note, this table does not have to be exhaustive. Dataset users and documentation consumers at large
are highly encouraged to contribute known usages.

#### Application(s)
<!-- scope: telescope -->
<!-- info: Provide a table of known AI/ML systems
that use this dataset.
-->

| **Application**           | **Brief Description**        | **Purpose of Dataset Usage**                           | **[AI Act Risk](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai)** |
|---------------------------|------------------------------|--------------------------------------------------------|----------------------------------------------------------------------------------------------|
| [Example Application 1]() | Size and Fit Recommendations | Fairness Evaluation of end to end application pipeline | Limited                                                                                      |


### Access
#### Relevant Links
* [Link to filestore]
* [Link to governance processes for data access]
* ...

## Access, Retention, and Deletion
==Patrick: header level of this is suddenly 2, all the others are 3.==
==Patrick does not know what this is about.  Data perhaps?==
<!-- info: NEEDS INPUT FROM PRIV-GOV! -->
### Access
#### Relevant Links
* [Link to filestore]
* [Link to governance processes for data access]
* ...

#### Data Security Classification 
<!-- scope: telescope -->
<!-- info: Select **one**: Use your companies data access classification
standards (replace the classifications below accordingly) -->
- C1
- C2
- C3
- C4
- Others (please specify)

#### Prerequisite(s)
<!-- scope: microscope -->
<!-- info: Please describe any required training or prerequisites to access
this dataset. -->
For example:

This dataset requires membership in [specific] database groups:

- Complete the [Mandatory Training]
- Read [Data Usage Policy]
- Initiate a [Data Processing Request]
- Get AWS IAM role with S3 bucket access
- Add Databricks cluster or other technical users to correct roles

### Retention
#### Duration
<!-- scope: periscope -->
<!-- info: Specify the duration for which this dataset can be retained: -->
Specify duration in days, months, or years.

#### Reasons for Duration
<!-- scope: periscope -->
<!-- info: Specify the reason for duration for which this dataset can be retained: -->
**Reason**

#### Policy Summary
<!-- scope: microscope -->
<!-- info: Summarize the retention policy for this dataset. -->
**Policy:** Add a link to the policy if it's standardized at your company (i.e. S3 bucket standard retention policies).

  
## Provenance
==Patrick: again level 2==
### Collection
#### Method(s) Used
<!-- scope: telescope -->
<!-- info: Select **all applicable** methods used to collect data.

Note on crowdsourcing, this covers the case where a crowd labels data
(make sure the reference the [Annotations and Labeling](#annotations-and-labeling)
section), or the case where a crowd is responsible for collecting and
submitting data independently to form a collective dataset.
-->
- API
- Artificially generated
- Crowdsourced - Internal Employee
- Crowdsourced - External Paid
- Crowdsourced - Volunteer
- Vendor collection efforts
- Scraped or crawled
- Survey, forms, or polls
- Interviews, focus groups
- Scientific experiment
- Taken from other existing datasets
- Unknown
- To be determined
- Others (please specify)

#### Methodology Detail(s)
<!-- scope: periscope -->
<!-- info: Provide a description of each collection method used.

Use additional notes to capture any other relevant information or
considerations.

(Usage Note: Duplicate and complete the following for collection method
type.) -->
**Collection Type**

**Source:** Describe here. Include links where available.

**Platform:** [Platform Name], Describe platform here. Include links where relevant.

**Is this source considered sensitive or high-risk?** [Yes/No]

**Dates of Collection:** [MMM YYYY - MMM YYYY]

**Update Frequency for collected data:**

*Usage Note: Select one for this collection type.*

- Yearly
- Quarterly
- Monthly
- Biweekly
- Weekly
- Daily
- Hourly
- Static
- Others (please specify)

**Additional Links for this collection:**

See section on [Access, Rention, and Deletion](#access-retention-and-deletion)

**Additional Notes:** Add here

#### Source Description(s)
<!-- scope: microscope -->
<!-- info: Provide a description of each upstream source of data.

Use additional notes to capture any other relevant information or
considerations. -->
- **Source:** Describe here. Include links, data examples, metrics, visualizations where relevant.
- **Source:** Describe here. Include links, data examples, metrics, visualizations where relevant.
- **Source:** Describe here. Include links, data examples, metrics, visualizations where relevant.

**Additional Notes:** Add here

#### Collection Cadence
<!-- scope: telescope -->
<!-- info: Select **all applicable**: -->
**Static:** Data was collected once from single or multiple sources.

**Streamed:** Data is continuously acquired from single or multiple sources.

**Dynamic:** Data is updated regularly from single or multiple sources.

**Others:** Please specify

  


### 4.1 Model Overview

**Model Name:**
**Model Type:** (e.g., Neural Networks, Decision Trees, etc.)
**Framework/Tools Used:**
#### Template Version
<!-- scope: telescope -->
<!-- info: link to model card version - we recommend using git tags / releases -->
[0.2.2]()

**Training Dataset:** (Reference dataset details)
**Development Timeframe:**
#### Model Overview
* Description
<!-- info: Brief (max 200 words) description of the model architecture and the task(s) it was trained to solve. -->

#### Status
<!-- scope: telescope -->
<!-- info: Select **one:** -->
**Status Date:** DD/MM/YYYY

**Under Preparation** - The model is still under active development
and is not yet ready for use due to active "dev" updates.

**Regularly Updated** - New versions of the model
have been or will continue to be made available.

**Actively Maintained** - No new versions will be made
available, but this model will
be actively maintained.

**Limited Maintenance** - The model will not be updated,
but any technical issues will be
addressed.

**Deprecated** - This model is obsolete or is
no longer being maintained.

### Developers
- **Name, Team**
- **Name, Team**

### Owners
<!-- info: Remember to reference developers and owners emails. -->
- **Team Name, Contact Person**

### Risk classification

<!-- info: Use the AI Act risk classification criteria found here: http://ai-act.eu/risk.
Reference assesment document if possible. -->
- High / Limited / Minimal

### Version Details and Artifacts
<!-- scope: periscope -->
<!-- info: Provide details about the current model version
and which model version the current model card corresponds to.

For models without version number, use "Not currently tracked"
but be sure to track the release date of the model.
-->
**Current Model Version:**

**Model Version Release Date:**

**Model Version for last Model Card Update:**

**Artifacts:**


- Model weights (e.g. S3 bucket path)
- Model config (e.g. S3 bucket path)

#### Github
<!-- info: Remember to link repositories. -->
- Repository_1
- Repository_2


#### 4.2 Model Purpose



#### Intended Use and Known Applications
#### Intended Use
<!-- info: This section focuses on the initial purpose and/or reasoning
for creating the model.-->

* Description

#### Domain(s) of use
* Description

**Specific tasks performed:**

#### Known Applications
<!-- info: Fill out the following section if the model has any
current known usages.
-->

| **Application**   | **Purpose of Model Usage**                                                 | **[AI Act Risk](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai)** |
|-------------------|----------------------------------------------------------------------------|----------------------------------------------------------------------------------------------|
| [Application 1]() | Foundation model providing customer embeddings for fraud detection scoring | High                                                                                         |
| [Application 2]() | Customer embeddings used directly as features for recommendation engine    | Limited                                                                                      |

Note, this table may not be exhaustive.  Model users and documentation consumers at large
are highly encouraged to contribute known usages.

#### Out Of Scope Uses
Provide potential applications and/or use cases for which use of the model is not suitable.


#### 4.3 Model Architecture

- Architecture Description:
    

- Key components
    
- Hyperparameters
    

- Training Methodology:
    

- Training duration
    
- Compute resources used
    

#### 4.4 Performance Metrics

- Evaluation Metrics Used: (e.g., Accuracy, Precision, Recall, AUC-ROC)
    
- Benchmarking Results:
    
- Validation Process:
    
- Real-World Performance:
    

- Stress testing
    
- Performance across different environments and populations
    

  
  
  

#### 4.5 Model Bias and Fairness Analysis

  

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXclauxwg1nWuPj2z0TcgUK9y69AqHzk_-jQ5BJwYeDkjPSOLVddFcHJ6-oOiuZ2p4Rk3VpqyKw9CvU7N1LOqYtpdjN6CV_hhTxTtpNj4auLmqhsaIQ5fRLIPnVpZOnhtR63YNELlg?key=Lv0_1kRp5_LSkJabUJ8gjQ)Implicit Bias, Measurement Bias, Temporal Bias, Selection Bias, Confounding Bias

#### Bias Detection Methods Used:
    

**Preprocessing:** Resampling, Reweighting,Transformation (data imputation, changing order of data); Relabeling, Blinding
    
**In-processing:** Transfer learning, Reweighting, Constraint optimization, Adversarial Learning, Regularization, Bandits
    
**Post-processing:** Transformation, Calibration, Thresholding
    

  

**Results of Bias Testing:**
    

#### Mitigation Measures:
    

**Fairness adjustments:** Introduce fairness criteria (like demographic parity, equal opportunity, or equalized odds) into the model training process. 
    
**Adversarial Debiasing:** Use adversarial networks to remove biased information during training. The main model tries to make accurate predictions, while an adversary network tries to predict sensitive attributes from the model's predictions.
    

#### Retraining approaches: 

**Fairness Regularization:** Modify the model's objective function to penalize bias. This introduces regularization terms that discourage the model from making predictions that disproportionately affect certain groups.
    
**Fair Representation Learning:** Learn latent representations of the input data that remove sensitive attributes, ensuring that downstream models trained on these representations are fair.
    
Post-Processing Techniques:

**Fairness-Aware Recalibration:** After the model is trained, adjust decision thresholds separately for different demographic groups to reduce disparities in false positive/false negative rates.
    
**Output Perturbation:** Introduce randomness or noise to model predictions to make outcomes more equitable across groups.
    
**Fairness Impact Statement:** Explain trade-offs made to satisfy certain fairness criterias
    

#### 4.6 Model Interpretability and Explainability

**Explainability Techniques Used:**
    

- Shapley values, LIME, etc.
    
**Post-hoc Explanation Models**

  

- Feature Importance (Permutation Importance, SHAP (SHapley Additive exPlanations), LIME (Local Interpretable Model-agnostic Explanations):
    
- Partial Dependence Plots (PDP)
    
- Counterfactual Explanations
    
- Surrogate Models
    
- Attention Mechanisms (for Deep Learning)
    

  

**Model-Specific Explanation Techniques**

  

- Grad-CAM (Gradient-weighted Class Activation Mapping)
    
- Layer-wise Relevance Propagation (LRP)
    
- TreeSHAP (SHAP for Decision Trees)
    

  
  

How interpretable is the model’s decision-making process?
    

  

Some technical tools that can aid transparency include:

- Data Lineage Tools: Track the flow and transformation of data (e.g., Apache Atlas, Pachyderm).
    
- Explainability Libraries: SHAP, LIME, Captum, TensorFlow Explain.
    
- Model Debugging Tools: What-If Tool, IBM AI Explainability 360.
    
- Version Control Systems: Git, DVC (Data Version Control) for datasets and models.
    

  
  
### Risk Management System

<!--**Instructions:**  A thorough risk management system is mandated by the AI Act, especially for high-risk AI systems. This section documents the  proactive efforts to ensure the AI system operates safely and ethically.-->


 **Risk Assessment Methodology:**  Describe the frameworks or standards used to identify and assess risks, such as ISO 31000 or failure mode and effects analysis (FMEA), or NIST Risk Assessment Framework.

 **Identified Risks:** 

  **Potential Harmful Outcomes:** List possible negative effects, such as biased decisions, privacy breaches, or safety hazards.

 **Likelihood and Severity:** Assess how likely each risk is to occur and the potential impact on users or society.

####Risk Mitigation Measures:

 **Preventive Measures:** Detail actions taken to prevent risks, like implementing data validation checks or bias reduction techniques.

 **Protective Measures:** Describe contingency plans and safeguards in place to minimize the impact if a risk materializes.

### Testing and Validation (Accuracy, Robustness, Cybersecurity)

**Testing and Validation Procedures (Accuracy):**

 **Performance Metrics:** List the metrics used to evaluate the AI system, such as accuracy, precision, recall, F1 score, or mean squared error.

 **Validation Results:** Summarize the outcomes of testing, including any benchmarks or thresholds met or exceeded.

**Measures for Accuracy:** High-quality data, algorithm optimisation, evaluation metrics, and real-time performance tracking.

  
#### Accuracy throughout the lifecycle:

**Data Quality and Management:** High-Quality Training Data: Data Preprocessing, techniques like normalisation, outlier removal, and feature scaling to improve data consistency, Data Augmentation, Data Validation

**Model Selection and Optimisation:** Algorithm selection suited for the problem, Hyperparameter Tuning (grid search, random search, Bayesian optimization), Performance Validation( cross-validation by splitting data into training and testing sets, using k-fold or stratified cross-validation), Evaluation Metrics (precision,recall, F1 score, accuracy, mean squared error (MSE), or area under the curve (AUC). 

**Feedback Mechanisms:** Real-Time Error Tracking, Incorporate mechanisms to iteratively label and include challenging or misclassified examples for retraining.

#### Robustness

**Robustness Measures:**

- Adversarial training, stress testing, redundancy, error handling, and domain adaptation.

**Scenario-Based Testing:**
- Plan for adversarial conditions, edge cases, and unusual input scenarios.
    
- Design the system to degrade gracefully when encountering unexpected inputs.
    

**Redundancy and Fail-Safes:**
    
- Introduce fallback systems (e.g., rule-based or simpler models) to handle situations where the main AI system fails.
    
**Uncertainty Estimation:**
    
- Include mechanisms to quantify uncertainty in the model’s predictions (e.g., Bayesian networks or confidence scores).
    

  

#### Cybersecurity

These measures include threat modelling, data security, adversarial robustness, secure development practices, access control, and incident response mechanisms.

Post-deployment monitoring, patch management, and forensic logging are crucial to maintaining ongoing cybersecurity compliance.

Documentation of all cybersecurity processes and incidents is mandatory to ensure accountability and regulatory conformity.

  

### Human Oversight

**Human-in-the-Loop Mechanisms:**  Explain how human judgment is incorporated into the AI system’s decision-making process, such as requiring human approval before action.

**Override and Intervention Procedures:** Describe how users or operators can intervene or disable the AI system in case of errors or emergencies.

 **User Instructions and Training:**  Provide guidelines and training materials to help users understand how to operate the AI system safely and effectively.

  **Limitations and Constraints of the System:** Clearly state what the AI system cannot do, including any known weaknesses or scenarios where performance may degrade.

  


  
  
  
