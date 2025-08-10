# Data Documentation Template 

<div style="color:gray">
  EU AI Act <a href="https://artificialintelligenceact.eu/article/10/" style="color:blue; text-decoration:underline">Article 10</a>
  <br>EU AI Act <a href="https://artificialintelligenceact.eu/article/11/" style="color:blue; text-decoration:underline">Article 11</a> ; <a href="https://artificialintelligenceact.eu/annex/4/" style="color:blue; text-decoration:underline">Annex IV</a> paragraph 1, 2 (d)
  <!-- info: The AI Act delineates the data governance practices required in Article 10 and requires a description of the intended purpose, version and provider, and relevant versions and updates.  
  In Article 11(2)(d), a datasheet is required which describes all training methodologies and techniques as well as the characteristics of the training dataset, a general description of the dataset, information about its provenance, scope and main characteristics, how the data was obtained and selected, labelling procedures conducted, and data cleaning methodologies deployed. -->
  <p></p>
</div>

**Dataset Owner**: Name and contact information
<br>**Document Version**: Version controlling this document is highly recommended
<br>**Reviewers**: List reviewers

<!-- info: Replace with dataset name -->

## Overview 
<!-- info: This section enables all stakeholders to have a glimpse into the data processes. You can use this session to provide transparency to users and high level information to all relevant stakeholders. -->

### Dataset Description 

<div style="color:gray">
  EU AI Act <a href="https://artificialintelligenceact.eu/article/11/" style="color:blue; text-decoration:underline">Article 11</a> ; <a href="https://artificialintelligenceact.eu/annex/4/" style="color:blue; text-decoration:underline">Annex IV</a> paragraph 1, 2(d)
  <p></p>
  <!-- info: The AI Act requires a description of  all training methodologies and techniques as well as the charatcteristics of the training dataset, general description of the dataset, information about their provenance, scope and main characteristics, how the data was obtained and selected labelling procedures conducted and data cleaning methodologies deployed.-->
</div>


Write a short summary describing your dataset (limit
200 words). Include information about the content
and topic of the data, sources and motivations for the
dataset, benefits and the problems or use cases it is
suitable for. For readers that only take 10 seconds to look
at this data card, adding one good overview image might also
make the difference between this data being discovered
and going unnoticed.

For more tips on describing data, see Zalando Data Foundation's
[Quality of Data Descriptions](https://docs.google.com/document/d/1njN1HMnNUl2J3aaY99FMwdJrSp0eMPsTY_cgOSsh46U)!<!-- info: Brief (max 200 words) description of the model architecture and the task(s) it was trained to solve. -->

### Status
<!-- scope: telescope -->
<!-- info: Select **one:** -->
**Status Date:** YYYY-MM-DD

**Status:** _specify one of_:

* **Under Preparation** -- The dataset is still under active curation and is not yet ready for use due to active "dev" updates.
* **Regularly Updated** -- New versions of the dataset have been or will continue to be made available.
* **Actively Maintained** -- No new versions will be made available, but this dataset will be actively maintained, including but not limited to updates to the data.
* **Limited Maintenance** -- The data will not be updated, but any technical issues will be addressed.
* **Deprecated** -- This dataset is obsolete or is no longer being maintained.

### Relevant Links
<!-- info: User studies show document users find quick access to relevant artefacts like papers, model demos, etc..
very useful. -->

Example references:

* GitHub Repository
* Paper/Documentation Link
* Initiative Demo
* Conference Talk
* API Link


### Developers

* **Name, Team**
* **Name, Team**

### Owner
<!-- info: Remember to reference developers and owners emails. -->
* **Team Name, Contact Person**

### Deployer instructions of Use
<!-- info: Important to determine if there are relevant use-cases or if the data is unsuitable for certair applications. -->
* **Instructions for use for deployers**:

<!-- 
How to use the data responsibly. Include restrictions, review process, ethical concerns. -->

<div style="color:gray">
  EU AI Act <a href="https://artificialintelligenceact.eu/article/13/" style="color:blue; text-decoration:underline">Article 13</a>
  <p></p>
</div>

### Version Details

## Data Versioning 

(Article 11, paragraph 2(d))

**Data Version Control Tools:**
<!-- Data version control tools are important to track changes in datasets, models, and experiments over time, enabling collaboration, reproducibility, and better model management. This is particularly important to then detect model drifts and debugging or for rollbacks when overwriting on the original data  -->

* Include a Data_versioning.md file to document changes
* DVC (Data Version Control): Tracks datasets, connects them to model versions, and integrates with Git.
* Git-LFS (Large File Storage): Stores large data files outside the Git repository.

### Maintenance of Metadata and Schema Versioning 

<div style="color:gray">
  EU AI Act <a href="https://artificialintelligenceact.eu/article/11/" style="color:blue; text-decoration:underline">Article 11</a> ; <a href="https://artificialintelligenceact.eu/annex/4/" style="color:blue; text-decoration:underline">Annex IV</a> paragraph 3
  <p></p>
</div>

#### Why

Data formats, schema, and other metadata changes can impact downstream processes. Tracking these ensures transparency.

#### How

Create a data dictionary:

* Document dataset structure, column descriptions, data types, and relationships.

Track schema changes:

* Use tools to log schema evolution.
* Record changes as part of version control or data pipelines.

 Save metadata alongside datasets:

* Include details like source, timestamp, description, version, and quality metrics.
    
  <!-- What could help is to incorporate Data Lineage Tools
   as they provide end-to-end visibility of data transformations and dependencies.-->

## Known Usages 

<div style="color:gray">
  EU AI Act <a href="https://artificialintelligenceact.eu/article/11/" style="color:blue; text-decoration:underline">Article 11</a> ; <a href="https://artificialintelligenceact.eu/annex/4/" style="color:blue; text-decoration:underline">Annex IV</a> paragraph 3
  <p></p>
  <!--info: The AI Act requires delineating a system’s foreseeable unintended outcomes and sources of risks to health and safety, fundamental rights, and discrimination in view of the intended purpose of the AI system;  
  the human oversight measures needed in accordance with Article 14, including the technical measures put in place to facilitate the interpretation of the outputs of AI systems by the deployers;  
  and specifications on input data, as appropriate.-->
</div>

<!-- info: Fill out the following section if the dataset has any
current known usages. This is important to make sure that the dataset is used ethically and legally. A dataset created for classification may not be suitable for regression, or vice versa.
Moreover, labeling quality, data coverage, and structure vary with use case—assuming it can be used for anything is dangerous. For instance:A skin lesion dataset created for classification—labeling images as benign, malignant, or uncertain—is mistakenly used by an insurance company to train a regression model that predicts cancer risk scores. Because the dataset lacks continuous risk-related data such as treatment outcomes, progression timelines, or cost indicators, the model produces unreliable predictions. As a result, high-risk patients may be misclassified as low-risk, leading to denied or delayed insurance claims. This misuse not only puts patients at risk but also exposes the insurer to ethical and legal scrutiny. Hence it is important to define the safe extent of use of a dataset. 
-->
### Model(s)
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

### Application(s)
<!-- scope: telescope -->
<!-- info: Provide a table of known AI/ML systems
that use this dataset.
-->

| **Application**           | **Brief Description**        | **Purpose of Dataset Usage**                           | 
|---------------------------|------------------------------|--------------------------------------------------------|
| [Example Application 1]() | Size and Fit Recommendations | Fairness Evaluation of end-to-end application pipeline |

## Dataset Characteristics

<div style="color:gray">
  EU AI Act <a href="https://artificialintelligenceact.eu/article/11/" style="color:blue; text-decoration:underline">Article 11</a> ; <a href="https://artificialintelligenceact.eu/annex/4/" style="color:blue; text-decoration:underline">Annex IV</a> paragraph 2(d)
  <p></p>
</div>
<!-- This section reflects the requirements of the AI Act of Article 11, paragraph 2 (d): where relevant, the data requirements in terms of datasheets describing the training methodologies and
techniques and the training data sets used, including a general description of these data sets, information about
their provenance, scope and main characteristics; how the data was obtained and selected; labelling procedures
(e.g. for supervised learning), data cleaning methodologies (e.g. outliers detection). Moreover, in order to comply with GDPR provisions, you need to disclose whether you are handling personal information. -->

**Data Types:** (e.g., images, text, audio, structured, unstructured data, personal data)
<br>**Size/Volume:**
<br>**Number of Instances/Records:**
<br>**Primary Use Case(s):** Description of the main AI use cases that the dataset was designed for or is typically used in.
<br>**Associated AI System(s):** List known AI system(s) that this dataset is or has been used in.
<br>**Number of Features/Attributes (if applicable):**
<br>**Label Information (if applicable):**
<br>**Geographical Scope:** Geographic location(s) where the data was collected.
<br>**Date of Collection:** Start and end date of data collection.

## Data Origin and Source
<!-- importanto to define this step to understand also compliance with GDPR.  -->
**Source(s):** Provide information about where the data was sourced from (e.g.,public datasets, sensors, surveys, web scraping, crowdsourced).
<br>**Third-Party Data:** Indicate if any part of the dataset was obtained from third parties, and if so, detail the legal agreements in place (license, usage rights, etc.).
<br>**Ethical Sourcing:** <!-- importanto to define this step to understand also compliance with GDPR.   -->Provide information on the ethical and legal compliance of the data collection process (e.g., informed consent, transparency to data subjects, and compliance with GDPR or other regulations).

## Provenance

_Describe the history and origin of the data._

### Collection

#### Method(s) Used
<!-- scope: telescope -->
<!-- info: Select **all applicable** methods used to collect data.

Note on crowdsourcing, this covers the case where a crowd labels data
(make sure the reference the [Annotations and Labeling](#annotations-and-labeling)
section), or the case where a crowd is responsible for collecting and
submitting data independently to form a collective dataset.
-->
_Specify one or more of:_

* API
* Artificially generated
* Crowdsourced - Internal Employee
* Crowdsourced - External Paid
* Crowdsourced - Volunteer
* Vendor collection efforts
* Scraped or crawled
* Survey, forms, or polls
* Interviews, focus groups
* Scientific experiment
* Taken from other existing datasets
* Unknown
* To be determined
* Others (please specify)

#### Methodology Detail(s) 

<div style="color: gray">
  EU AI Act <a href="https://artificialintelligenceact.eu/article/11/" style="color:blue; text-decoration:underline">Article 11</a> ; <a href="https://artificialintelligenceact.eu/annex/4/" style="color:blue; text-decoration:underline">Annex IV</a> 2 (a), (b), (d)
  <p></p>
</div>
<!-- scope: periscope -->
<!-- info: Provide a description of each collection method used. Use additional notes to capture any other relevant information or
considerations. (Usage Note: Duplicate and complete the following for collection method
type.) -->
**Collection Type**

**Source:** Describe here. Include links where available.

**Platform:** [Platform Name], Describe platform here. Include links where relevant.

**Is this source considered sensitive or high-risk?** [Yes/No]

**Dates of Collection:** [YYYY-MM -- YYYY-MM]

**Update Frequency for collected data:**

_Select one for this collection type:_ yearly, quarterly, monthly, on demand, no changes, others, ....

**Additional Links for this collection:**

See section on [Access, Rention, and Deletion](#access-retention-and-deletion)

**Additional Notes:** Add here

#### Source Description(s)
<!-- scope: microscope -->
<!-- info: Provide a description of each upstream source of data.

Use additional notes to capture any other relevant information or
considerations. -->
* **Source:** Describe here. Include links, data examples, metrics, visualizations where relevant.
* **Source:** Describe here. Include links, data examples, metrics, visualizations where relevant.
* **Source:** Describe here. Include links, data examples, metrics, visualizations where relevant.

**Additional Notes:** Add here

#### Collection Cadence
<!-- scope: telescope -->
<!-- info: Select **all applicable**: -->
**Static:** Data was collected once from single or multiple sources.

**Streamed:** Data is continuously acquired from single or multiple sources.

**Dynamic:** Data is updated regularly from single or multiple sources.

**Others:** Please specify
    
## Data Pre-Processing 

<div style="color:gray">
  EU AI Act <a href="https://artificialintelligenceact.eu/article/11/" style="color:blue; text-decoration:underline">Article 11</a> ; <a href="https://artificialintelligenceact.eu/annex/4/" style="color:blue; text-decoration:underline">Annex IV</a> paragraph 2 (d, e)
  <p></p>
</div>

### Data Cleaning

* Handling missing data: (e.g., removal, imputation method used)
* Outlier treatment: (e.g., detection and removal technique)
* Duplicates removal: (Yes/No)
* Error correction: (Manual/Automated, if applicable)

### Data Transformation

* Normalization/Standardization: (Method used, e.g., min-max scaling)
* Encoding categorical data: (e.g., one-hot encoding, label encoding)
* Text/tokenization: (Applicable for NLP tasks)

### Feature Engineering

* Feature selection: (e.g., methods used to select features)
* Feature extraction: (e.g., PCA, interaction terms)
* Newly created features: (List any)

### Dimensionality Reduction

* Technique(s) used: (e.g., PCA, t-SNE)
* Number of dimensions after reduction: (Specify)

### Data Augmentation

* Augmentation technique(s): (e.g., rotation, flipping for images)

## Data Annotation and Labeling 

<div style="color: gray">
  EU AI Act <a href="https://artificialintelligenceact.eu/article/11/" style="color:blue; text-decoration:underline">Article 11</a> ; <a href="https://artificialintelligenceact.eu/annex/4/" style="color:blue; text-decoration:underline">Annex IV</a> 2(d)
  <p></p>
</div>

* Annotation Process: Describe the process used to label or annotate the data (e.g., human labelers, automated, crowdsourcing).
* Annotation platform
* Validation: Explain any quality control mechanisms applied to ensure accurate labeling or annotation
  - Inter-Annotator agreement
  - Consensus process
  - Calibration rounds

* Annotator Demographics (Location / Language / Expertise / Background)

## Validation Types

### Method(s) 

Example= range and constraint validation, structured validation, consistency validation

### Breakdown(s)

**(Validation Type)**

**Number of Data Points Validated:** 

### Description(s)


## Sampling Methods


### Method(s) Used


### Characteristic(s)

### Sampling Criteria



### Description(s)

## Dataset Distribution and Licensing 

<div style="color: gray">
  EU AI Act <a href="https://artificialintelligenceact.eu/article/11/" style="color:blue; text-decoration:underline">Article 11</a> ; <a href="https://artificialintelligenceact.eu/annex/4/" style="color:blue; text-decoration:underline">Annex IV</a> 2(d)
  <p></p>
</div>

* Availability:
* Open/public or private dataset
* Dataset Documentation Link: (Link to further details if available)
* User Rights and Limitations:

## Access, Retention, and Deletion
<!-- info: Where applicable, collect input from privacy governance team -->
### Access

#### Relevant Links

* [Link to filestore]
* [Link to governance processes for data access]
* ...

#### Data Security Classification in and out of scope delineation
<!-- scope: Is there a potentially harmful application iof this data, can you foresee this?  -->
<!-- info: Select **one**: Use your companies data access classification
standards (replace the classifications below accordingly) -->


#### Prerequisite(s)
<!-- scope: microscope -->
<!-- info: Please describe any required training or prerequisites to access
this dataset. -->
For example:

This dataset requires membership in [specific] database groups:

* Complete the [Mandatory Training]
* Read [Data Usage Policy]
* Initiate a [Data Processing Request]

### Retention

#### Duration
<!-- scope: periscope -->
<!-- info: Specify the duration for which this dataset can be retained: -->
Specify duration in days, months, or years.

#### Reasons for Duration
<!-- scope: periscope -->
<!-- info: Specify the reason for duration for which this dataset can be retained: -->
...

#### Policy Summary
<!-- scope: microscope -->
<!-- info: Summarize the retention policy for this dataset. -->
**Policy:** Add a link to the policy if it's standardized at your company 
  
## Data Risk Assessment

**Describe the assessment of data risks**:

* Foreseeable unintended outcomes or biases arising from dataset use.
* Sources of potential discrimination or harm.


## Cybersecurity Measures

<div style="color: gray">
  EU AI Act <a href="https://artificialintelligenceact.eu/article/11/" style="color:blue; text-decoration:underline">Article 11</a> ; <a href="https://artificialintelligenceact.eu/annex/4/" style="color:blue; text-decoration:underline">Annex IV</a> paragraph 5
  <p></p>
</div>


### Data Security Measures

#### Data Storage

* **Encryption**: Use AES-256; detail key management (e.g., HSM, key rotation).
* **Access Control**: Implement role-based access and MFA.
* **Backup**: Document backup frequency, encryption, and recovery testing.
* **Integrity Monitoring**: Use hashes, checksums, or blockchain.
* **Security**: Describe server protections (e.g., restricted access).

#### Data Transfer

* **Encryption in Transit**: Specify TLS 1.3, IPsec configurations.
* **Endpoint Security**: Detail device verification and certificate pinning.
* **API Security**: Document authentication, rate-limiting, and channel encryption.
* **Data Masking**: Use pseudonymisation for sensitive data in transit.

#### Data Processing

* **Secure Environments**: Use containers, VMs, or trusted execution (e.g., Intel SGX).
* **Audit Logs**: Specify logging standards, retention, and tamper protection.
* **Data Minimisation**: Anonymise or limit collected data.



### Standards Applied
 <!-- info: provide information of the standards applied and certifications in this section-->

### Data post-market monitoring

-**Data Drift Detection and Monitoring:** Describe here what type of drift was identified (covariate drift, prior probability drift or concept drift)

<!-- info: This section is particularly important as it enables to understand whether the model is still making accurate predictions, especially if used in critical domains. 
For instance: If yoi train a model to detec and diagnose lung cancer from hospital A, deploying to hopsital B might affect accuracy as the other hospital might use different scanning machines that have different contrasts or resolutions and therefore might affect the distributional differences of the input images and the model might drop accuracy.
 .-->

-**Audit Logs:** Periodically perform manual or semi-automated reviews of data samples and log changes in the data as well as access patterns.

* **Action plans implemented to address identified issues:**.



### EU Declaration of conformity

<div style="color: gray">
  EU AI Act <a href="https://artificialintelligenceact.eu/article/47/" style="color:blue; text-decoration:underline">Article 47</a>
  <p></p>
</div>

 <!-- when applicable and certifications are available: it requires a systems name as well as the name and address of the provider; a statement that the EU declaration of conformity referred to in Article 47 is issued under the sole responsibility of the provider; a statement that the AI system is in conformity with this Regulation and, if applicable, with any other relevant Union law that provides for the issuing of the EU declaration of conformity referred to in Article 47, Where an AI system involves the processing of personal data;  a statement that that AI system complies with Regulations (EU) 2016/679 and (EU) 2018/1725 and Directive (EU) 2016/680, reference to the haharmonised standards used or any other common specification in relation to which
conformity is declared; the name and identification number of the notified body, a description of the conformity
assessment procedure performed, and identification of the certificate issued; the place and date of issue of the declaration, the name and function of the person who signed it, as well as an
indication for, or on behalf of whom, that person signed, a signature.-->

### Standards applied
<!-- Document here the standards and frameworks used-->


### Documentation Metadata

### Version
<!-- info: provide version of this document, if applicable (dates might also be useful) -->

### Template Version
<!-- info: link to model documentation template (i.e. could be a GitHub link) -->

### Documentation Authors
<!-- info: Give documentation authors credit

Select one or more roles per author and reference author's
emails to ease communication and add transparency. -->

* **Name, Team:** (Owner / Contributor / Manager)
* **Name, Team:** (Owner / Contributor / Manager)
* **Name, Team:** (Owner / Contributor / Manager)
