# 1. Introduction

Postie, Inc ("Postie") is committed to ensuring the confidentiality, privacy, integrity, and availability of all electronic protected health information (ePHI) it receives, maintains, processes and/or transmits on behalf of its Customers. As providers of compliant, hosted applications used by health technology enterprises, Postie strives to maintain compliance, proactively address information security, mitigate risk for its Customers, and assure known breaches are completely and effectively communicated in a timely manner. The following documents address core policies used by Postie to maintain compliance and assure the proper protections of infrastructure used to store, process, and transmit ePHI for Postie Customers.

Postie provides secure and compliant cloud-based software. This hosted software falls into a broad category: 1) **Software as a Service (Saas)**.

## 1.1 Software as a Service (SaaS)

SaaS Customers utilize hosted software and infrastructure from Postie to model, deploy, and measure direct mail and potentially other marketing campaigns. This software is deployed into compliant containers run on systems secured and managed by Postie. Postie makes every effort to reduce the risk of unauthorized disclosure, access, and/or breach of SaaS Customer data through network (firewalls, dedicated IP spaces, etc) and server settings (encryption at rest and in transit, etc).

## 1.2 Compliance Inheritance

Postie provides compliant hosted software infrastructure for its Customers. Postie's service offerings are available on AWS.

Postie signs business associate agreements (BAAs) with its Customers. These BAAs outline Postie obligations and Customer obligations, as well as liability in the case of a breach. In providing infrastructure and managing security configurations that are a part of the technology requirements that exist in HIPAA and HITRUST, as well as future compliance frameworks, Postie manages various aspects of compliance for Customers. The aspects of compliance that Postie manages for Customers are inherited by Customers, and Postie assumes the risk associated with those aspects of compliance. In doing so, Postie helps Customers achieve and maintain compliance, as well as mitigates Customers risk.

Certain aspects of compliance cannot be inherited. Because of this, Postie Customers, in order to achieve full compliance or HITRUST Certification, must implement certain organizational policies. These policies and aspects of compliance fall outside of the services and obligations of Postie.

## 1.3 Postie Organizational Concepts

The physical infrastructure environment is hosted at [Amazon Web Services](https://aws.amazon.com/) (AWS). The network components and supporting network infrastructure are contained within the infrastructures and managed by AWS. Postie does not have physical access into the network components. The Postie environment consists of nginx and Puma web servers; Ruby application servers; Redshift and PostgreSQL database servers;  logging servers; Linux Ubuntu  servers; Machine Learning environments on EC2 and EMR, and developer tool servers running on Linux Ubuntu.

Within the Postie Platform on AWS, all data transmission is encrypted and relevant hard drives, S3 storage, and SSD drives are encrypted so that PHI data at rest is also encrypted.

In the case of SaaS Customers, it is the responsibility of the Customer to restrict, secure, and assure the privacy of all ePHI data at the User Level, as this is not under the control or purview of Postie. This includes not sharing login credentials to the Postie system with users who are not authorized to view PHI.

Application servers and load balancers are externally facing and accessible via the Internet. The database servers, where the ePHI resides, are located on the internal Postie network and can only be accessed through a bastion host (SSH Jump Machine). Access to the internal database is restricted to a limited number of personnel and strictly controlled to only those personnel with a business-justified reason. Remote access to internal servers is not accessible except through SSH key-only login.


## 1.4 Requesting Audit and Compliance Reports

Postie, at its sole discretion, shares audit reports with customers on a case by case basis. All audit reports are shared under explicit NDA in Postie format between Postie and party to receive materials. Audit reports can be requested by Postie workforce members for Customers or directly by Postie Customers.

## 1.6 Version Control

A full version history of these policies is available upon request.
