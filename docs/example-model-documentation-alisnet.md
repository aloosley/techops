# ALiSNet Model Documentation

**Model Owner**: [Amrollah Seifoddini]()
<br>**Document Version**: 0.2.0
<br>**Reviewers**: [Alex Loosley](), [Rocco Maresca]()

Model documentation contributions and feedback are welcome!

## Overview

### Model Type

Convolutional Neural Network

### Model Description
<!-- info: Brief (max 200 words) description of the model architecture and the task(s) it was trained to solve. -->
**A**ccurate and **Li**ghtweight mobile human **S**egmentation **Net**work (ALiSNet) is a Convolutional Neural Network (CNN) for semantic segmentation of human silhouettes from photos.
Architecture of ALiSNet is based on [Semantic FPN](https://arxiv.org/abs/1901.02446) with [PointRend](https://arxiv.org/abs/1912.08193) refinement. The original backbone of the network is exchanged by mobile-optimized [MnasNet](https://arxiv.org/abs/1807.11626) to achieve significant model size reduction. Additionaly, Feature Pyramid Network (FPN) from the original backbone is replaced with a simpler aggregation step, skipping FPN top-down path. Final model is also quantized to 8 bits integer precision using Qantization Aware Training.

### Status

**Status Date:** 2025-01-22

**Regularly Updated** - New versions of the model have been or will continue to be made available.

### Relevant Links

* [Paper](https://arxiv.org/abs/2304.07533)

### Developer(s)

[**Amrollah Seifoddini**](), **Size & Fit**

### Owner(s)
<!-- info: Remember to reference developers and owners emails. -->
**Team Name**: [**Size & Fit**]()

**Contact Person**: [**Amrollah Seifoddini**]()

## Version Details and Artifacts
<!-- scope: periscope -->
<!-- info: Provide details about the current model version
and which model version the current model card corresponds to.

For models without version number, use "Not currently tracked"
but be sure to track the release date of the model.
-->
**Current Model Version:** Not currently tracked

**Model Version Release Date:** N/A

**Model Version for last Model Card Update:** N/A

**Artifacts:**

## Intended and Known Usage
<!-- info: The model owners are not expected to track all applications that use this model.-->
### Intended Use
<!-- info: This section focuses on the initial purpose and/or reasoning
for creating the model.-->

Model was developed to perform semantic segmentation of humans vs. background as a step in inference of body 
measurements from photos. Given the specific use case, 
ALiSNet was trained to work for very narrow arm and leg angles ranges.

### Out of Scope Uses

ALiSNet was trained to work for very narrow arm and leg angles ranges. It shouldn't be used for general semantic segmentation tasks of human silhouettes vs. background.

### Known Applications
<!-- info: Fill out the following section if the model has any
current known usages.
-->

| **Application**                                                                                                                          | **Purpose of Model Usage**                                                                    | **[AI Act Risk](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai)** |
|------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------|
| [Body Measurements Pipeline](https://docs.google.com/document/d/1bJKJR43o285XEiiThrx4xtqwzXl2bbu3SThUNy7Rbic/edit#heading=h.a6wkeijjbx1) | ALiSNet is used for silhouette extraction as part of Size & Fit's Body Measurements Pipeline. | Limited                                                                                      |

Note, this table may not be exhaustive.  Model users and documentation consumers at large
are highly encouraged to contribute known usages.

## Risks and Ethical Considerations

Privacy risks were initially reviewed by Size & Fit ([J. Peterman](), [Frank Constanza](), [David Puddy](), [Stefan Messmer]()) in collaboration with Algorithmic Privacy & Fairness ([Elaine Benes]()) and Product Security ([Kenny Bania]()).

### Processing or storage of customer photos during deployment

In order to obtain measurments customers need to upload their photos to our app so that their silhouette may be inferred. This creates a risk related to storage and processing of private data.

**Mitigation strategy:**

ALiSNet is deployed on-device. Customers photos are processed and stored on their device and Zalando does not have access to them. Only inferred silhouettes are sent to Zalando servers.

### On-device deployment

Deploying ALiSNet on-device may cause risks related to backdoor attacks against ML models such as Membership Inference or Model Inversion which may result in violation of privacy of our customers.

**Mitigation strategy:**

[Privacy risk assessment](https://docs.google.com/document/d/1OXFrcyWblFIHLw9uOXsla8e-zBhtFwlgIBH84MdvrrM/edit?usp=sharing) was performed in order to quantify Membership Inference (MIA) risk of the ALiSNet.
As of November 2022 results of the audit showed that MIA risk is none to low.

### Biases in model performance

Statistically relevant discrepancies in the model accuracy across protected attributes related to human characteristics such as age, percieved skin tone, height etc..

**Mitigation Strategy:**

[Fairnes assessment](https://docs.google.com/presentation/d/1DhjDdjWzgIkkjhVg1-AM9VzibCK27kW1kpUEDim3CMA/edit?usp=sharing) was performed in order to qunatify potential discerpancies across derived skin tone and body shape.
As of October 2022 no relevant discrepencies in model performance were found.

## Training
<!-- info: This section should include overview regarding training process such as training dataset(s), training task (ex. next token prediciton, pixel-wise classification). -->
ALiSNet is a classification model trained on semantic segmentation task which goal is to perform a classification of pixels in the input image with corresponding semantic class (human, bike etc.).

See [ALiSNet Paper](https://arxiv.org/abs/2304.07533) for more details about training.

### Datasets

| Name                                                              | Location                                | Sensitive* | Size         |   
|-------------------------------------------------------------------|-----------------------------------------|------------|--------------|
| Filtered Common Objects in Context (COCO)                         | s3://sagemaker-io-2/coco/               | No*        | ~50k samples |
| Another Production Dataset Training Split (Another Dataset Train) | s3://obfuscated-bucket-name/production/ | Yes*       | 3625 samples |

(*): Requires a special Data Processing Request


## Evaluation
<!-- info: Remember to reference metrics definitions and results variance (if available.) -->
See [ALiSNet Paper](https://arxiv.org/abs/2304.07533) for more details about testing such as performance metrics and baselines.

### Performance Metrics

Metrics used to evaluate model:

* **MIoU**: [Mean Intersection over Union](https://en.wikipedia.org/wiki/Jaccard_index)

**Results**:

* Voices of Customers (VOC):
  * **MIoU**: 97.6 (+/- 0.1)

### Model Bias and Fairness Analysis

See [Body Measurement Prediction Fairness Paper](https://ceur-ws.org/Vol-3442/paper-17.pdf) for complete fairness assessment results.

### Datasets

ALiSNet was evaluated using multiple datasets. All of the datasets represent realistic examples expected to be seen in intended deployment scenario.

| Name                                                                           | Location                                           | Sensitive* | Size         |
|--------------------------------------------------------------------------------|----------------------------------------------------|------------|--------------|
| Faces dataset<sup>1</sup>                                                      | s3://obfuscated-bucket-name/faces/production/      | Yes*       | 2416 samples |
| Voices of Customers (VOC) dataset<sup>1,2</sup>                                | s3://obfuscated-bucket-name/voc/production/        | Yes*       | 6494 samples |
| Optimass dataset<sup>1</sup>                                                   | s3://obfuscated-bucket-name/optimass/production/   | Yes*       | 322 samples  |
| [Skin tones dataset](example-data-documentation-voc-skin-tones.md)<sup>2</sup> | s3://obfuscated-bucket-name/skin-tones/production/ | Yes*       | 499 samples  |

(*): Requires a special Data Processing Request
<br>(1): Used for overall performance evaluation
<br>(2): Used for fairness evaluation

## Caveats and Recommendations

Poor lightning conditions and low photo resolution may decrease quality of segmentation. (?)

The model was designed with strong size and latency constraints and is ready to be deployed to production or edge devices.

## Documentation Metadata

Note, some names in this document have been anonymized.

### Documentation Template Version

[v1.0.0](template-model-documentation.md)

### Documentation Authors

* **[Rocco Maresca](), Algorithmic Privacy & Fairness:** (Owner)
