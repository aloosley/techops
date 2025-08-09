# Home

## TechOps Introduction

* Are you looking for guidance on how to create technical documentation for your AI/ML system 
  and/or its constituent models and datasets?  
* Should your AI/ML system documentation provide value to a wide variety of user personas 
  (managers, system users, developers, researchers, regulators, etc.)?
* Does your AI/ML system need to comply with the EU AI Act, or are you developing a model or dataset that
  you want to be used as part of an AI/ML system that needs to comply with the EU AI Act?

If you answered yes to any of these questions, TechOps is for you.  

TechOps, published in [AIES 2025](https://www.aies-conference.com/2025/) (see [citation details](#citing) below), 
is a set of documentation templates and examples designed to help technical teams and companies
document their AI/ML applications, models, and datasets. TechOps is also the first set of documentation 
templates that we know of to completely map its sections to the EU AI Act, for developers and providers 
that need to comply with this regulation that first came into force in August 2024.

While the primary contribution of TechOps is documentation guidance and examples, we also recognize that not every user already has an approach to rendering their documentation to maximize its value in the real world to a wide variety of personas (managers, system users, developers, researchers, regulators, etc.).  Therefore, we also provide a [blueprint for rendering your own TechOps Documentation]. The TechOps documentation examples seen on this very website are rendered using this blueprint.

See [Getting Started](#getting-started) below for more details.

## Citing

If you use and parts of this work, we kindly ask that you cite our paper:

```bibtex
@inproceedings{lucaj2025techops,
   title     = {TechOps: Technical Documentation Templates for the AI Act},
   author    = {Laura Lucaj and Alex Loosley and H{\aa}kan Jonsson and Urs Gasser and Patrick van der Smagt},
   booktitle = {Proceedings of the Eighth {AAAI/ACM} Conference on AI, Ethics, and Society {(AIES-25)}},
   publisher = {{AAAI} Press},
   year      = {2025}
}
```

## Templates

TechOps are three separate templates for sufficiently documenting AI systems for proof of compliance with the AI Act.
The documentation is split into three levels:

* AI System documentation
* Model documentation
* Data documentation

to allow the owners of data, models, and AI systems to each maintain ownership of their own level of documentation.  
Thus, model and dataset owners whom may or may not have curated their models and datasets with a specific AI Systems in 
mind, may still create documentation contributions that the AI System documentation can reference.

These templates are meant to guide responsible stakeholders to document AI systems across various fields. 
Unlike existing lengthy and abstract questionnaires, these templates offer clear guidance for the documentation of the 
relevant processes across the AI lifecycle, translating complex requirements such as fairness and data governance 
into actionable metrics and measurable criteria that can be implemented and tracked. 
This process ensures that the abstract legal requirements of the AI Act are operationalized into concrete actions, 
making them manageable and measurable.

Following the TechOps approach also provides stakeholders comprehensive oversight on the data, model and application lifecycle. These templates track the system’s status over the 
entire AI lifecycle, ensuring traceability, reproducibility, in addition to compliance with the AI Act. 

Clear documentation also promotes discoverability, collaboration, and risk assessment.

## Examples

The templates are tested on real-world scenarios providing examples that further guide their implementation:

|                                                                            | Description                                                                                                                                                     | 
|----------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [Application Documentation Example](example-application-documentation-safesite-ai.md) | SafeSiteAI is a **fictional** high-risk AI system developed to detect and monitor construction worker safety using real-time video analytics and sensor fusion. | 
| [Model Documentation Example](example-model-documentation-alisnet.md)      | A neural network for segmenting human silhouettes in photos                                                                                                     |
| [Data Documentation Example](example-data-documentation-voc-skin-tones.md) | A skin tones dataset created to support fairness evaluations of downstream computer vision models and human centric applications like SafeSiteAI                |

## Getting Started

Developing TechOps documentation is easy, it's just markdown!  Simply create your own markdown files following the [TechOps Documentation Templates](#templates) (For template files, see our [GitHub Page](https://github.com/aloosley/techops)).

How you render your TechOps Documentation is up to you, but we also provide a blueprinted approach for rendering TechOps documentation.  To use it, follow the instructions on our [GitHub Page](https://github.com/aloosley/techops).
