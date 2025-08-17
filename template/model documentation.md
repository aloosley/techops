# Model Documentation Template
<!-- info: Replace with model name -->

<div style="color:gray">
    EU AI Act <a href="https://artificialintelligenceact.eu/article/11/" style="color:blue; text-decoration:underline">Article 11</a>, paragraph 1
    <!-- info:  
    The AI Act requires a description of  
    (a) the intended purpose, version, and provider,  
    (b) a description of how the system interacts with software and hardware,  
    (c) relevant versions and updates,  
    (d) all the forms in which the AI system is put into service
    The overview part should also include:  
    (e) the hardware on which the system is intended to run,  
    (f) whether the system is part of the safety component of a product,  
    (g) a basic description of the user interface, and  
    (h) the instructions for use for the deployers. 
    -->
    <p></p>
</div>

**Model Owner**: Name and contact information
<br>**Document Version**: Version controlling this document is highly recommended
<br>**Reviewers**: List reviewers

## Overview 

<div style="color:gray">
EU AI Act <a href="https://artificialintelligenceact.eu/article/11/" style="color:blue; text-decoration:underline">Article 11</a>, paragraph 1

<!-- info: This section enables all stakeholders to have a glimpse into the model selection, design, and development processes.  
You can use this section to provide transparency to users and high-level information to all relevant stakeholders.-->
<p></p>
</div>

### Model Type

**Model Type:** (e.g., Neural Networks, Decision Trees, etc.)

### Model Description 

<div style="color:gray">
    EU AI Act <a href="https://artificialintelligenceact.eu/article/11/" style="color:blue; text-decoration:underline">Article 11</a> ; <a href="https://artificialintelligenceact.eu/annex/4/" style="color:blue; text-decoration:underline">Annex IV</a>  paragraph 1(a)
    <p></p>
</div>

* Description
<!-- info: Brief (max 200 words) description of the model architecture and the task(s) it was trained to solve, architecture (e.g., FPN, PointRend, MnasNet), size/latency optimization, and intended purpose. -->

### Status 
<!-- scope: telescope -->
<!-- info: Select **one:** -->
**Status Date:** YYYY-MM-DD

**Status:** _specify one of_:

* **Under Preparation** -- The model is still under active development and is not yet ready for use due to active "dev" updates.
* **Regularly Updated** -- New versions of the model have been or will continue to be made available.
* **Actively Maintained** -- No new versions will be made available, but this model will be actively maintained.
* **Limited Maintenance** -- The model will not be updated, but any technical issues will be addressed.
* **Deprecated** -- This model is obsolete or is no longer being maintained.

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

## Version Details and Artifacts 

<div style="color:gray">
    EU AI Act <a href="https://artificialintelligenceact.eu/article/11/" style="color:blue; text-decoration:underline">Article 11</a> ; <a href="https://artificialintelligenceact.eu/annex/4/" style="color:blue; text-decoration:underline">Annex IV</a> paragraph 1(c)
    <p></p>
</div>

<!-- scope: periscope -->
<!-- info: Provide details about the current model version
and which model version the current model card corresponds to.

For models without version number, use "Not currently tracked"
but be sure to track the release date of the model.
-->


**Current Model Version:**

**Model Version Release Date:**

**Model Version at last Model Documentation Update:**

**Artifacts:**

* Model weights (e.g. S3 bucket path)
* Model config <!-- (s3://your-bucket/path/to/config.yaml)-->

## Intended and Known Usage

### Intended Use
<!-- info: This section focuses on the initial purpose and/or reasoning
for creating the model. It is important to define this section as the intended use directly affects the AI Act classification. For example:
A face recognition model for personal photo apps → Limited risk
The same model used for law enforcement → High or unacceptable risk


Example Use Case: A university research team develops a machine learning model to predict the likelihood of hospital readmission among diabetic patients over the age of 65, using data from a regional healthcare network. The model is trained and validated specifically on this elderly population and is intended to support hospital planning and academic research. However, the team does not document the model’s intended use or demographic limitations. A health-tech company later integrates the model into a mobile app aimed at helping diabetes patients of all ages manage their care. The model performs poorly for younger users, frequently overestimating their risk of readmission. This leads to unnecessary anxiety, inappropriate self-care decisions, and false alerts to care providers. The misapplication draws criticism for lacking transparency, and regulators question the ethics of deploying a model outside its original context.   -->

* Description

### Domain(s) of use

* Description


**Specific tasks performed:**

 **Instructions for use for deployers**:
<div style="color:gray">
    EU AI Act <a href="https://artificialintelligenceact.eu/article/11/" style="color:blue; text-decoration:underline">Article 13</a> ; <a href="https://artificialintelligenceact.eu/annex/4/" style="color:blue; text-decoration:underline">Annex IV</a> 
    <p></p>
</div>

### Out Of Scope Uses

Provide potential applications and/or use cases for which use of the model is not suitable.

### Known Applications 

<div style="color:gray">
    EU AI Act <a href="https://artificialintelligenceact.eu/article/11/" style="color:blue; text-decoration:underline">Article 11</a> ; <a href="https://artificialintelligenceact.eu/annex/4/" style="color:blue; text-decoration:underline">Annex IV</a>  paragraph 1(f)
    <p></p>
</div>

<!-- info: Fill out the following section if the model has any
current known usages.
-->

| **Application**   | **Purpose of Model Usage**                                                 | **[AI Act Risk](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai)** |
|-------------------|----------------------------------------------------------------------------|----------------------------------------------------------------------------------------------|
| [Application 1]() | Foundation model providing customer embeddings for fraud detection scoring | High                                                                                         |
| [Application 2]() | Customer embeddings used directly as features for recommendation engine    | Limited                                                                                      |

Note, this table may not be exhaustive.  Model users and documentation consumers at large
are highly encouraged to contribute known usages.

## Model Architecture 

<div style="color:gray">
EU AI Act <a href="https://artificialintelligenceact.eu/article/11/" style="color:blue; text-decoration:underline">Article 11</a>; <a href="https://artificialintelligenceact.eu/annex/4/" style="color:blue; text-decoration:underline">Annex IV</a>  paragraph 2(b), 2(c)

Info – AI Act requirements:  
This section should contain a description of the elements of the model and the processes of its training and development.  

Article 11(2)(b) requires the design specifications of a system, model selection, and what the system is designed to optimize for, as well as potential trade-offs.  

Article 11(2)(c) requires a description of the system’s architecture, how software components are built on or feed into each other, and the computational resources needed to develop, train, test, and validate the system.
</div>


<!-- Info: Describing the architecture is fundamental for reproducibility, transparency, and effective maintenance. Without clear records of the model’s layers, activation functions, input/output shapes, and training configurations, it becomes difficult to reproduce results, debug issues, or update the model reliably.  -->


* Architecture Description

* Key components
    
* Hyperparameter tuning methodology

* Training Methodology

* Training duration
    
* Compute resources used
    

### Data Collection and Preprocessing

<div style="color:gray">
    EU AI Act <a href="https://artificialintelligenceact.eu/article/11/" style="color:blue; text-decoration:underline">Article 11</a>; <a href="https://artificialintelligenceact.eu/annex/4/" style="color:blue; text-decoration:underline">Annex IV</a>  paragraph 2(d)
    <p></p>
</div>

<!--check data documentation to avoid duplicates of information and link it in this sectiion

In Article 11, 2 (d) a datasheet is required which describes all training methodologies and techniques as well as the characteristics of the training dataset, general description of the dataset, information about their provenance, scope and main characteristics, how the data was obtained and selected labelling procedures conducted and data cleaning methodologies deployed -->

* **Steps Involved**:
  * Data collection: Describe how the data was sourced (e.g., databases, APIs, sensors, or publicly available datasets).
  * Data cleaning: Explain techniques used to handle missing values, outliers, or errors.
        
  * Data transformation: Include any scaling or encoding applied.


       
### Data Splitting 

* **Subset Definitions**:
  * **Training set**: 
  * **Validation set**: 
  * **Test set**: 
* **Splitting Methodology**:
  * Describe the approach:
    * **Random Sampling**: 
    * **Stratified Sampling**: 
    * **Temporal Splits**: 
* **Proportions**:
  * Example: "70% training, 20% validation, 10% testing."
* **Reproducibility**:
  * Mention how many seeds are being used and how many are needed to prove statistical significance
    
**Data Shuffling**:

* Shuffle applied: (Yes/No) 

## Model Training Process 

<div style="color:gray">
    EU AI Act <a href="https://artificialintelligenceact.eu/article/11/" style="color:blue; text-decoration:underline">Article 11</a> ; <a href="https://artificialintelligenceact.eu/annex/4/" style="color:blue; text-decoration:underline">Annex IV</a>  paragraph 2(c, g), paragraph 3

<!-- AI Act requirements info:  
In Article 11 paragraph 2(c), details about the computational resources needed to develop, train, test, and validate AI systems are required.  

Moreover, in accordance with Article 11 paragraph 2(g), this section must include the validation and testing procedures used, the data involved, and the main metrics adopted to measure accuracy, robustness, and compliance with the requirements laid out in Chapter III, Section 2.  

Paragraph 3 further requires detailed information about the monitoring, functioning, and control of the system, as well as logging of testing, with reports dated and signed by responsible stakeholders.-->
<p></p>
</div>


**Details of Processes**:

* **Initialisation**: 
* **Loss Function**:
* **Optimiser**:
* **Hyperparameters**:
        
## Model Training and Validation 

<div style="color:gray">
    EU AI Act <a href="https://artificialintelligenceact.eu/article/11/" style="color:blue; text-decoration:underline">Article 11</a> ; <a href="https://artificialintelligenceact.eu/annex/4/" style="color:blue; text-decoration:underline">Annex IV</a>  paragraph 2(g)
    <br>EU AI Act <a href="https://artificialintelligenceact.eu/article/11/" style="color:blue; text-decoration:underline">Article 15</a>
    <p></p>
</div>

Objective: Clarify what the model is supposed to achieve. 

* Problem statement (e.g., classification of X, prediction of Y)
* Business goals (accuracy, fairness, speed)
* Metrics selected (e.g., accuracy, precision, recall, F1-score, AUC-ROC, MAE, RMSE)
Rationale for each metric (why accuracy? why F1-score?)

* Model predictions on the validation set evalutaion description. 

<!--
- Performance metrics (e.g., accuracy, F1 score, RMSE) are monitored.
- Documeting this step is important as it enables to detect errors and performance issues early on: Overfitting can be detected using validation loss trends.
-->

<!--### Performance Metrics

- Evaluation Metrics Used (e.g., Accuracy, Precision, Recall, AUC-ROC)
- Benchmarking Results
- Validation Process
- Real-World Performance
- Stress testing
- Performance across different environments and populations -->

**Hyperparameter Tuning**:
    

        
**Regularisation**:
    

    
**Early Stopping**:
    

## Model Testing and Evaluation

<!--
- Performance metrics (e.g., accuracy, F1 score, RMSE) are monitored.
- Documeting this step is important as it enables to detect errors and performance issues early on: Overfitting can be detected using validation loss trends.
-->

<!-- Example: In medical diagnosis, using accuracy alone can be misleading in imbalanced datasets, potentially missing critical cases like cancer. Metrics like recall (which measures the percentage of actual cancer cases the model correctly identifies. Critical for minimizing missed diagnoses), precision ( to ensure that when the model predicts cancer, it’s actually correct—important to reduce false alarms), F1 score, and AUC-ROC provide a more meaningful assessment by accounting for the real-world impact of false positives and false negatives. Choosing the right metrics ensures models are effective, trustworthy, and aligned with practical goals and consequences.

## Model Validation and Testing
- **Assess the metrics of model performance** 
   - accuracy:
   - precision: 
   - recall:
   - F1 score:

- **Advanced performance metrics**
  - ROC-AUC:
    - trade-off between true positive rate and false positive rate
  - PR- AUC
     - Evaluating precision and recall trade-off
  - Specificity
    - (True Negatives/(True Negatives+False Positives))
  - Log Loss (Cross-Entropy Loss):
    - Penalises incorrect probabilities assigned to classes.


- **Context dependant metrics**: 
  - Regression Metrics: For tasks predicting continuous values
  - Clustering Metrics: for tasks grouping similar data points
  - Ranking Metrics: for tasks predicting rankings (e.g., search engines recommendation systems)
  - NLP processing metrics (e.g., text classification, sequence-to-sequence tasks)


- **Fairness Metrics**:
    
    - Ensure the model treats different groups (e.g., based on gender, race) equitably.
    - Examples: Demographic parity, equal opportunity, and disparate impact.
- **Explainability Metrics**:
    
    - Measure how understandable and interpretable are the model’s decisions.
    - Examples: Feature importance, fidelity (how well explanations match the model), and sparsity (using fewer features for explanations).
    - 
- **Robustness Metrics**:
    
    - Assess how well the model performs under challenging or unexpected conditions.
    - Examples: Adversarial robustness, performance under data drift, and sensitivity to input changes.
 
- Limitations of the performance after the tests
- Simulate deployment scenarios to understand real-world implications.
- Define thresholds for acceptable performance levels.
- Justify the choice of metrics based on the application’s purpose.
   
--> 

 **Performance Metrics**:
    
* Compute metrics on the test set:
  * Accuracy, precision, recall, F1 score for classification.
  * MSE, RMSE, MAE for regression.

 **Confusion Matrix**:
    
* Generate a confusion matrix to evaluate classification results.

 **ROC Curve and AUC**:
    
* For binary classifiers, compute the ROC curve and Area Under the Curve (AUC).

 **Feature Importance**:
    
* Analyse feature contributions (for explainability).

 **Robustness Testing**:

* Test the model on edge cases or adversarial examples.

 **Comparison to Baselines**:
    
* Compare the model’s performance to a simple baseline (e.g., random guess, mean prediction).

### Model Bias and Fairness Analysis 

<div style="color:gray">
    EU AI Act <a href="https://artificialintelligenceact.eu/article/11/" style="color:blue; text-decoration:underline">Article 11</a> ; <a href="https://artificialintelligenceact.eu/annex/4/" style="color:blue; text-decoration:underline">Annex IV</a>  paragraph 2 (f, g), paragraph 3, 4
    <p></p>
</div>

<!-- info: This section aims to cover the AI Act requirements layed out in Article 11 paragraph 2 g that requires the description of the potential discriminatory impacts. 
Paragraph 4 requires the assessment of the appropriateness of the performance metrics.-->  



![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXclauxwg1nWuPj2z0TcgUK9y69AqHzk_-jQ5BJwYeDkjPSOLVddFcHJ6-oOiuZ2p4Rk3VpqyKw9CvU7N1LOqYtpdjN6CV_hhTxTtpNj4auLmqhsaIQ5fRLIPnVpZOnhtR63YNELlg?key=Lv0_1kRp5_LSkJabUJ8gjQ)Implicit Bias, Measurement Bias, Temporal Bias, Selection Bias, Confounding Bias

#### Bias Detection Methods Used
    

**Pre-processing:** Resampling, Reweighting,Transformation (data imputation, changing order of data); Relabeling, Blinding
    
**In-processing:** Transfer learning, Reweighting, Constraint optimization, Adversarial Learning, Regularization, Bandits
    
**Post-processing:** Transformation, Calibration, Thresholding
    


**Results of Bias Testing:**
    

#### Mitigation Measures
    

**Fairness adjustments:** Introduce fairness criteria (like demographic parity, equal opportunity, or equalized odds) into the model training process. 
    
**Adversarial Debiasing:** Use adversarial networks to remove biased information during training. The main model tries to make accurate predictions, while an adversary network tries to predict sensitive attributes from the model's predictions.
    

#### Retraining approaches

**Fairness Regularization:** Modify the model's objective function to penalize bias. This introduces regularization terms that discourage the model from making predictions that disproportionately affect certain groups.
    
**Fair Representation Learning:** Learn latent representations of the input data that remove sensitive attributes, ensuring that downstream models trained on these representations are fair.
    
### Post-Processing Techniques

**Fairness-Aware Recalibration:** After the model is trained, adjust decision thresholds separately for different demographic groups to reduce disparities in false positive/false negative rates.
    
**Output Perturbation:** Introduce randomness or noise to model predictions to make outcomes more equitable across groups.
    
**Fairness Impact Statement:** Explain trade-offs made to satisfy certain fairness criterias
    

## Model Interpretability and Explainability 

<div style="color:gray">
    EU AI Act <a href="https://artificialintelligenceact.eu/article/11/" style="color:blue; text-decoration:underline">Article 11</a>; <a href="https://artificialintelligenceact.eu/annex/4/" style="color:blue; text-decoration:underline">Annex IV</a>  paragraph 2(e)
    <p></p>
</div>

**Explainability Techniques Used:**
  <!-- for example: Shapley values, LIME, etc. Both SHAP and LIME are explainability techniques that help to understand why a machine learning model made a specific prediction — especially when the model is a complex "black box" like a random forest, gradient boosting, or deep neural net. Shap Uses game theory to assign each feature a value showing how much it contributed to a prediction. Lime builds a simple, interpretable model (like a linear model) near the point of interest to explain the prediction -->
    
  Examples: 
    SHAP (SHapley Additive exPlanations), 
    LIME (Local Interpretable Model-agnostic Explanations)

**Post-hoc Explanation Models**

* Feature Importance, Permutation Importance, SHAP (SHapley Additive exPlanations), LIME (Local Interpretable Model-agnostic Explanations):
* Partial Dependence Plots (PDP) 
* Counterfactual Explanations
* Surrogate Models
* Attention Mechanisms (for Deep Learning)
    

**Model-Specific Explanation Techniques**

<!-- info: this part is important to delineate why a model makes a decision or to debug and identify if the model is focusing on the right parts of the input. Especially fundamental for models deployed in critical domains such as medical, financial and legal or law enforcement. This section can be useful to draft the user-interface section of the documentation.) -->

* Grad-CAM (Gradient-weighted Class Activation Mapping) for CNNs and RNNs: especially for computer vision applications 
* Layer-wise Relevance Propagation (LRP): Works well for CNNs, fully connected nets, and some RNNs (classification focused)
* TreeSHAP (SHAP for Decision Trees)
    

How interpretable is the model’s decision-making process? 


<!--
Some technical tools that can aid transparency include:
- Data Lineage Tools: Track the flow and transformation of data (e.g., Apache Atlas, Pachyderm).
- Explainability Libraries: SHAP, LIME, Captum, TensorFlow Explain.
- Version Control Systems: Git, DVC (Data Version Control) for datasets and models. -->

### EU Declaration of conformity 

<div style="color:gray">
    EU AI Act <a href="https://artificialintelligenceact.eu/article/47/" style="color:blue; text-decoration:underline">Article 47</a>(d)
    <p></p>
</div>

 <!-- when applicable and certifications are available: it requires a systems name as well as the name and address of the provider; a statement that the EU declaration of conformity referred to in Article 47 is issued under the sole responsibility of the provider; a statement that the AI system is in conformity with this Regulation and, if applicable, with any other relevant Union law that provides for the issuing of the EU declaration of conformity referred to in Article 47, Where an AI system involves the processing of personal data;  a statement that that AI system complies with Regulations (EU) 2016/679 and (EU) 2018/1725 and Directive (EU) 2016/680, reference to the harmonised standards used or any other common specification in relation to which
conformity is declared; the name and identification number of the notified body, a description of the conformity
assessment procedure performed, and identification of the certificate issued; the place and date of issue of the declaration, the name and function of the person who signed it, as well as an
indication for, or on behalf of whom, that person signed, a signature.-->

### Standards applied

<!-- Document here the standards and frameworks used-->

## Documentation Metadata

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
