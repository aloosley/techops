# SafeSiteAI Application Documentation

**Application Owner**: [George Costanza](mailto:g.costanza@vandelay-industries.com), Vandelay Industries
<br>**Document Version**: 0.4.1
<br>**Reviewers**: [Jerry Seinfeld](), [Alex Loosley]()

## Relevant Links

* [GitHub Repository]()
* [Deployment Pipeline]()
* [API]() ([Swagger Docs]())
* [AWS Account]()
* [JIRA Backlog]()
* [LeanIX Page]()

## General Information

**Purpose and Intended Use**:
SafeSiteAI is a **fictional** high-risk AI system developed to detect and monitor construction worker safety using real-time video 
analytics and sensor fusion. The system's primary objective is to identify unsafe behaviors 
(e.g., not wearing PPE, entering danger zones) and hazardous conditions (e.g., falling debris, proximity to heavy machinery) to trigger alerts, prevent accidents, and support regulatory compliance.

* **Sector**: Construction and Occupational Safety
* **Problem Solved**: Reduces on-site accidents, improves compliance with safety protocols  
* **Target Users**: Site supervisors, safety managers, construction companies  
* **KPIs**: Reduction in incidents, response time to alerts, detection accuracy 
* **Ethical/Regulatory**: Adheres to GDPR for video data, complies with EU AI Act for high-risk systems
* **Prohibited Uses**: Employee surveillance beyond safety (e.g., productivity scoring) 
* **Operational Environment**: Deployed on-site with edge devices, synced with a cloud dashboard


## Risk Classification

* **Classification**: High 
* **Reasoning**: Monitors safety-critical scenarios in a workplace where human health is at risk, regulated under AI Act Article 6(1)(a) and (b)

## Application Functionality

* **Instructions for Use for Deployers**:
  * System requires regular calibration and access to camera feeds and IoT sensors.    
  * Alerts are issued via on-site monitors and mobile apps.
* **Model Capabilities**:
  * Detects PPE (helmets, vests), boundary breaches, fall incidents, and idle heavy machinery  
  * Limitations: Lower accuracy under poor lighting/weather conditions 
  * Languages supported: English, German
* **Input Data Requirements**:
  * Real-time video feeds (HD cameras), sensor logs
  * Valid inputs: stable camera angle, active worker zones   
  * Invalid inputs: occluded views, uncalibrated sensors
* **Output Explanation**:
  * Generates classification alerts (e.g., PPE violation) with confidence scores
  * Provides bounding box visualizations and timestamps
* **System Architecture Overview**:
  * See [SafeSiteAI LeanIX Architecture]()

## Models and Datasets

### Models

| Model                        | Documentation                                                    | Description of Application Usage                    |
|------------------------------|------------------------------------------------------------------|-----------------------------------------------------|
| ALiSNet                      | [TechOps Model Document](example-model-documentation-alisnet.md) | Used for identity masked human and PPE segmentation |
| PPE Fit and Usage Classifier | [TechOps Model Document]()*                                      | Used to score if PPE properly used                  |
| Other Danger Classifier      | [GitHub Repo]()*                                                 | Used to detect other safety hazards in view         |

* Fictional example (no link provided)

### Datasets

| Dataset             | Documentation                                                         | Description of Application Usage        |
|---------------------|-----------------------------------------------------------------------|-----------------------------------------|
| Skin tones dataset  | [TechOps Data Document](example-data-documentation-voc-skin-tones.md) | Used for end-to-end application testing |
| PPE annotation data | [GitHub Repo]()*                                                      | Used for end-to-end application testing |

* Fictional example (no link provided)

Note, other datasets were used to train, evaluate, and test [models](#models) used as part of SafeSiteAI. 
See those documentation for details about those datasets.

## Application Development

## Deployment

* **Cloud Setup**: See [LeanIX Page]()
* **APIs**: [Backend]() (see [Swagger Documentation]())  
* **Integration**: Application integrated into Vandelay Industries [SafeSiteAI Suite]() 

## Integration with External Systems

* **Systems**:
  * Dependencies: Camera hardware, sensor suite, on-site edge gateway
  * Data flow diagrams showing interactions: Site -> Edge Device -> Cloud -> Dashboard 
  * Error-handling mechanisms: Retry logic, manual fallback

## Deployment Plan

* **Infrastructure**:
  * Environments: development, staging, production  
  * Scaling: Auto-scale based on number of cameras 
  * Backup and recovery: Daily snapshots, recovery under 15 minutes
* **Integration Steps**:
  * Deploy pipeline: edge device → data store → alert engine → dashboard    
  * Dependencies: PyTorch, OpenCV, AWS SDK  
  * Rollback: Last-stable container with health-check triggers
* **User Information**: Currently deployed across 6 EU construction sites

## Lifecycle Management

* **Monitoring**:
  * Performance: Detection latency, accuracy (see [Grafana monitoring dashboard]())
  * Infrastructure: CPU, memory, network (see [Grafana monitoring dashboard]())
* **Versioning and change logs**: See Application [GitHub Repository]()  
* **Key Activities**:
  * [Continuous evaluation]()  
  * Retraining quarterly or on demand        
* **Documentation Needs**:
  * Logs: Accuracy drift  
  * Audit trails: [Model update logs]()
  * Incident reports: Alert false positives/negatives
        

## Risk Management System

* **Methodology**: ISO 31000 + Hazard Identification Matrix
* **Identified Risks**:
  * False negatives (undetected hazards) 
  * Privacy violations (video storage)
* **Mitigation**:
  * Preventive: Diverse [evaluation data](#datasets), [identity masking](#models) (ALiSNet)
  * Protective: Manual override, encrypted alert logs

## Testing and Validation (Accuracy, Robustness, Cybersecurity)

* **Accuracy**: See latest deployed model scores in [Model Registry]()
* **Robustness**: See latest deployed model scores in [Model Registry]()
* **Cybersecurity**:
  * TLS 1.3, IAM roles, intrusion logging
  * See [Monitoring Dashboard]()
        

## Human Oversight

* **Human-in-the-loop**: Required for alert validation 
* **Override**: Site manager may suppress or escalate alerts
* **Training**: Safety staff [trained]() on alert review interface
* **Limitations**: Cannot detect underground/chemical hazards - See [QA Board]() for more details
    

## Incident Management

* **Common Issues**:
  * False alarms from shadows/motion  
  * Compatibility issues with legacy hardware  
* **Support Contact**:
  * [24/7 tech hotline](), [escalation team]()
        

## EU Declaration of Conformity

* **System Name**: SafeSiteAI
* **Provider**: Vandelay Industries, New York, NY, 10101 USA
* **Compliance**: EU AI Act Art. 47, GDPR, ISO/IEC 27001

## Standards Applied

* ISO 31000: Risk Management 
* ISO/IEC 27001: Information Security
* IEC 61508: Functional Safety

See [Governance Approvals]() for more information

## Documentation Metadata

### Template Version

[Link to Template](template-application-documentation.md)

### Documentation Authors

- **[George Costanza](mailto:g.costanza@vandelay-industries.com), Importer/Exporter:** (Principal Developer)
