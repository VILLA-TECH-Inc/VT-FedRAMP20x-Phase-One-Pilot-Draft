# VT-FedRAMP20x-Phase-One-Pilot-Draft
<h2>CSO & CSP Summaries – Lightweight Documentation </h2> 

 

<h3>Villa-Tech, Inc.</h3> 
Villa-Tech, Inc. is a technology-driven Minority Business Enterprise specializing in cloud computing, cybersecurity, and IT infrastructure. The company is committed to delivering innovative solutions tailored to client needs while ensuring compliance with industry standards such as CMMC 2.0 Level 2, NIST 800-53 Revision 5, ISO 27001, and FedRAMP. Villa-Tech focuses on deploying scalable and secure cloud environments, implementing robust security measures to protect data and systems, and designing resilient IT infrastructures to support mission-critical operations. Their expertise includes Zero Trust Architecture (ZTA) and Cybersecurity Maturity Model Certification (CMMC) readiness, leveraging the NIST Risk Management Framework (RMF) for security reviews, assessments, remediation, audit preparation, and managed services. 

<h3>STRUCTURA.IO </h3>
STRUCTURA.IO is Villa-Tech’s flagship product, an AI-assisted, low-code platform designed to automate and streamline cloud infrastructure development, management, and security. It empowers organizations to build, plan, and deploy Infrastructure as Code (IaC) with ease, leveraging a drag-and-drop interface and full Terraform functionality. STRUCTURA.IO serves as a centralized control center for infrastructure needs, bridging the skill gap between experienced and novice users while supporting standardized workflows like GitOps and CI/CD pipelines. Key features include Zero Trust Architecture (ZTA) support, compliance automation, cost optimization, AI-driven automation, multi-cloud and edge support, Terraform integration, and security and scalability. STRUCTURA.IO is tailored to meet the needs of government and commercial organizations, offering robust solutions for compliance, data integration, and process automation, enhancing operational efficiency, and protecting sensitive data. 

<h2>KSI Validation & Evidence </h2>

This draft submission details the methodology for validating the suggested FedRAMP Key Security Indicators (KSIs). Each KSI defines a security goal and encompasses several validations to illustrate compliance. The Cloud Service Provider (CSP) will generate machine-readable assertions ("FULLY_IMPLEMENTED", "PARTIALLY_IMPLEMENTED", "NOT_IMPLEMENTED", "NOT_APPLICABLE") for every validation, in addition to a score that reflects the overall compliance for each KSI. Furthermore, a threshold value will be established for what qualifies as FULLY_IMPLEMENTED, PARTIALLY_IMPLEMENTED, NOT_IMPLEMENTED, or NOT_APPLICABLE. During our audit procedure, we plan to engage a 3PAO to authenticate the precision and purpose of each validation. This process will involve examining the validation logic and its corresponding KSI through traditional audit processes like interviews and walkthroughs. 
 
<h3>Sample KSI validation output</h3>

    "KSI-CMT": {
      "name": "Configuration Management and Templates",
      "status": "PARTIALLY_IMPLEMENTED",
      "score": 80,
      "evidence": [
        "Azure Automation DSC configuration",
        "Change tracking solution deployed",
        "Infrastructure as Code with Terraform"
      ],
      "findings": [
        {
          "severity": "MEDIUM",
          "finding": "Duplicate resource configuration detected in Terraform",
          "recommendation": "Remove duplicate local_file resource 'baseline_config_dsc'",
          "control_reference": "CM-2, CM-6"
        }
      ]
    }

<h2>Automation and Machine Readable Data Requirement</h2> 

Data Schema and full machine readable package found within these text files:
<ul>
 <li><a href="https://github.com/VILLA-TECH-Inc/VT-FedRAMP20x-Phase-One-Pilot-Draft/blob/main/KSI-validation-template.txt">KSI-validation-template.txt</a></li>
 <li><a href="https://github.com/VILLA-TECH-Inc/VT-FedRAMP20x-Phase-One-Pilot-Draft/tree/main/KSI-Results">KSI-Results folder</a></li>
</ul>

<h2>3PAO Review </h2>

We have proactively engaged with Third Party Assessment Organizations (3PAOs) to assist in completing a comprehensive assessment of our implementation of the FedRAMP 20X Low requirements and Key Security Indicators (KSIs). This engagement is crucial for ensuring that our security measures meet the stringent standards set by FedRAMP. By collaborating with 3PAOs, we aim to leverage their expertise to thoroughly evaluate our security protocols and validate our compliance with federal guidelines. 

Although we have yet to establish a working relationship with a 3PAO, once connected, we will work closely with them to rigorously validate our automated validation scheme for KSIs. This process involves a detailed examination of our security controls and mechanisms to ensure they are functioning correctly and effectively. 

<h2>Continuous Reporting Prototype</h2>

Our methodology for continuous reporting will leverage our proprietary cloud service, STRUCTURA.IO, to deliver a customer-facing dashboard that is updated daily with the results of Key Security Indicators (KSIs). This dashboard provides comprehensive insights by displaying the validation description, KSI name, KSI ID, result ("FULLY_COMPLIANT", "SUBSTANTIALLY_COMPLIANT", "PARTIALLY_COMPLIANT", "NON_COMPLIANT"), and the last run timestamp. By utilizing this approach, we ensure that our clients have real-time access to critical security metrics, enabling them to make informed decisions and maintain robust security postures. 


 

<h2>Methods and Summary </h2>

Our method for generating the machine-readable package involves utilizing our cloud service offering, STRUCTURA.IO, to generate a FedRAMP Moderate architecture for hosting our Cloud Service Offering (CSO). This robust architecture ensures compliance with stringent security standards. We then employ STRUCTURA.IO to generate the machine-readable package, leveraging the agent within our CSO to create the Key Security Indicator (KSI) validation template. This approach guarantees a secure and efficient process for producing the necessary validation templates, ensuring our clients receive reliable and accurate security metrics.
