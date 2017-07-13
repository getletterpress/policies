# 17. Data Integrity Policy

Postie takes data integrity very seriously. As stewards and partners of Postie Customers, we strive to assure data is protected from unauthorized access and that it is available when needed. The following policies drive many of our procedures and technical settings in support of the Postie mission of data protection.

Production systems that create, receive, store, or transmit Customer data (hereafter "Production Systems") must follow the guidelines described in this section.

## 17.1 Applicable Standards

### 17.1.1 Applicable Standards from the HITRUST Common Security Framework

* 10.b - Input Data Validation

### 17.1.2 Applicable Standards from the HIPAA Security Rule

* 164.308(a)(8) - Evaluation

## 17.2 Disabling Non-Essential Services

1. All Production Systems must disable services that are not required to achieve the business purpose or function of the system.

## 17.3 Monitoring Log-in Attempts

1. All access to Production Systems must be logged. This is done following the Postie Auditing Policy.

## 17.4 Prevention of Malware on Workstations

2. Virus scanning software is run on all workstations for anti-virus protection.

## 17.5 Patch Management

1. Software patches and updates will be applied to all systems in a timely manner.

## 17.6 Production System Security

1. System, network, and server security is managed and maintained by the CTO.
2. Access to Production AWS console is controlled using centralized tools and two-factor authentication.

## 17.7 Production Data Security

1. Reduce the risk of compromise of Production Data.
2. Implement and/or review controls designed to protect Production Data from improper alteration or destruction.
3. Ensure that confidential data is stored in a manner that supports user access logs and automated monitoring for potential security incidents.
4. Ensure Postie Customer Production Data is segmented and only accessible to Customer authorized to access data.


## 17.8 Transmission Security

1. All PHI data transmission is encrypted end to end using encryption keys managed by Postie.
2. Transmission encryption keys and machines that generate keys are protected from unauthorized access. Transmission encryption key material is protected with access controls such that the key material is only accessible by privileged accounts.