# 13. Disaster Recovery Policy

The Postie Contingency Plan establishes procedures to recover Postie following a disruption resulting from a disaster. This Disaster Recovery Policy is maintained by the Postie Security Officer and Privacy Officer.

The following objectives have been established for this plan:

1. Maximize the effectiveness of contingency operations through an established plan that consists of the following phases:
   * *Notification/Activation phase* to detect and assess damage and to activate the plan;
   * *Recovery phase* to restore temporary IT operations and recover damage done to the original system;
   * *Reconstitution phase* to restore IT system processing capabilities to normal operations.
2. Identify the activities, resources, and procedures needed to carry out Postie processing requirements during prolonged interruptions to normal operations.
3. Identify and define the impact of interruptions to Postie systems.
4. Assign responsibilities to designated personnel and provide guidance for recovering Postie during prolonged periods of interruption to normal operations.
5. Ensure coordination with other Postie staff who will participate in the contingency planning strategies.
6. Ensure coordination with external points of contact and vendors who will participate in the contingency planning strategies.

Example of the types of disasters that would initiate this plan are natural disaster, political disturbances, man made disaster, external human threats, internal malicious activities.

Postie defined two categories of systems from a disaster recovery perspective.

1. *Critical Systems*. These systems host application servers and database servers or are required for functioning of systems that host application servers and database servers. These systems, if unavailable, affect the integrity of data and must be restored, or have a process begun to restore them, immediately upon becoming unavailable.
2. *Non-critical Systems*. These are all systems not considered critical by definition above. These systems, while they may affect the performance and overall security of critical systems, do not prevent Critical systems from functioning and being accessed appropriately. These systems are restored at a lower priority than critical systems.

## 13.1 Applicable Standards

## 13.1.1 Applicable Standards from the HITRUST Common Security Framework

* 12.c - Developing and Implementing Continuity Plans Including Information Security

## 13.1.2 Applicable Standards from the HIPAA Security Rule

* 164.308(a)(7)(i) - Contingency Plan

## 13.2 Line of Succession

The following order of succession to ensure that decision-making authority for the Postie Contingency Plan is uninterrupted. The Chief Technology Officer (CTO) is responsible for ensuring the safety of personnel and the execution of procedures documented within this Postie Contingency Plan. If the CTO is unable to function as the overall authority or chooses to delegate this responsibility to a successor, the CEO or VPCX shall function as that authority. To provide contact initiation should the contingency plan need to be initiated, please use the contact list below.

* Jonathan Neddenriep, CTO: jonathan@Postie.com
* David Fink, CEO: d@Postie.com
* Tim Hamelen, VP-CX: 608-577-7003, tim@Postie.com

## 13.3 Responsibilities

The following teams have been developed and trained to respond to a contingency event affecting the IT system.

1. The **Ops Team** is responsible for recovery of the Postie hosted environment, network devices, and all servers. Members of the team include personnel who are also responsible for the daily operations and maintenance of Postie. The team leader is the CTO and directs the Dev Ops Team.
2. The **Web Services Team** is responsible for assuring all application servers, web services, and platform add-ons are working. It is also responsible for testing redeployments and assessing damage to the environment. The team leader is the CTO and directs the Web Services Team.

Members of the Ops and Web Services teams must maintain local copies of the contact information from [§13.2](#13.2-line-of-succession). Additionally, the CTO must maintain a local copy of this policy in the event Internet access is not available during a disaster scenario.

## 13.4 Disaster Recovery Procedures

### 13.4.1 Notification and Activation Phase

This phase addresses the initial actions taken to detect and assess damage inflicted by a disruption to Postie. Based on the assessment of the Event, sometimes according to the Postie Incident Response Policy, the Contingency Plan may be activated by either the CTO.

The notification sequence is listed below:

* The first responder is to notify the CTO. All known information must be relayed to the CTO.
* The CTO is to contact the Web Services Team and inform them of the event. The CTO is to to begin assessment procedures.
* The CTO is to notify team members and direct them to complete the assessment procedures outlined below to determine the extent of damage and estimated recovery time. If damage assessment cannot be performed locally because of unsafe conditions, the CTO is to follow the steps below.
  * Damage Assessment Procedures:
  * The CTO is to logically assess damage, gain insight into whether the infrastructure is salvageable, and begin to formulate a plan for recovery.
  * Alternate Assessment Procedures:
  * Upon notification, the CTO is to follow the procedures for damage assessment with combined Dev Ops and Web Services Teams.
* The Postie Contingency Plan is to be activated if one or more of the following criteria are met:
  * Postie will be unavailable for more than 48 hours.
  * Hosting facility is damaged and will be unavailable for more than 24 hours.
  * Other criteria, as appropriate and as defined by Postie.
  * If the plan is to be activated, the CTO is to notify and inform team members of the details of the event and if relocation is required.
  * Upon notification from the CTO, group leaders and managers are to notify their respective teams. Team members are to be informed of all applicable information and prepared to respond and relocate if necessary.
  * The CTO is to notify the hosting facility partners that a contingency event has been declared and to ship the necessary materials (as determined by damage assessment) to the alternate site.
  * The CTO is to notify remaining personnel and executive leadership on the general status of the incident.
  * Notification can be message, email, or phone.

### 13.4.2 Recovery Phase

This section provides procedures for recovering the application at an alternate site, whereas other efforts are directed to repair damage to the original system and capabilities.

The following procedures are for recovering the Postie infrastructure at the alternate site. Procedures are outlined per team required. Each procedure should be executed in the sequence it is presented to maintain efficient operations.

Recovery Goal: The goal is to rebuild Postie infrastructure to a production state.

The tasks outlines below are not sequential and some can be run in parallel.

1. Contact Partners and Customers affected - Web Services
2. Assess damage to the environment - Web Services
3. Begin replication of new environment
4. Test new environment - Web Services
5. Test logging, security, and alerting functionality - Dev Ops
6. Assure systems are appropriately patched and up to date. - Dev Ops
7. Deploy environment to production - Web Services
8. Update DNS to new environment. - Dev Ops

### 13.4.3 Reconstitution Phase

This section discusses activities necessary for restoring Postie operations at the original or new site. The goal is to restore full operations within 24 hours of a disaster or outage. When the hosted data center at the original or new site has been restored, Postie operations at the alternate site may be transitioned back. The goal is to provide a seamless transition of operations from the alternate site to the computer center.

1. Original or New Site Restoration
   * Begin replication of new environment using automated and tested scripts
   * Test new environment - Web Services
   * Test logging, security, and alerting functionality. - Dev Ops
   * Deploy environment to production - Web Services
   * Assure systems are appropriately patched and up to date. - Dev Ops
   * Update DNS to new environment. - Dev Ops
2. Plan Deactivation
   * If the Postie environment is moved back to the original site from the alternative site, all hardware used at the alternate site should be handled and disposed of according to the Postie Media Disposal Policy.
