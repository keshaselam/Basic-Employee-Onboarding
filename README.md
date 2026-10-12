## Problem Statement
During the initial assessment of Northstar Medical Group (NMG), I identified gaps in the Active Directory organizational structure, including missing departmental Organizational Units (OUs) for Finance, HR, IT, and Operations. The managed service provider (MSP) had not maintained consistent account management procedures, resulting in poor documentation, inconsistent provisioning, and delayed deprovisioning of user accounts. Inconsistent security group membership created the potential for excessive or insufficient access, leaving some employees with permissions beyond their job requirements while preventing others from accessing resources needed for their roles. These access control weaknesses increased the risk of unauthorized access to protected health information (PHI) and potential HIPAA compliance issues.

## Solution Overview
I established the NMG.com Active Directory domain using a Domain Controller to provide centralized identity management and authentication for the organization. I created four organizational units (OUs)—Finance, HR, IT, and Operations—to structure employee accounts by department and support organized directory administration. I created corresponding security groups (Finance-Users, HR-Users, IT-Users, and Operations-Users) to organize users and facilitate controlled access to department-specific resources. I designed a flat role-based access control (RBAC) model in which users receive baseline permissions through their assigned departmental security group, with additional access limited to approved job responsibilities and the principle of least privilege. For user provisioning, I recorded employee attributes, including name, SAM account name, user principal name (UPN), job title, and department, and configured temporary passwords to require a change at first logon. Provisioning security is evaluated through verification of authorization, appropriate group membership, password configuration, and assigned permissions, with validation and audit evidence documented for each account.

## Video Walkthrough
[Add your video walkthrough link placeholder here. You will record this tomorrow and update this link so visitors can see a live demonstration of your lab environment.]

## Tools Used
* Windows Server
* Active Directory Domain Services
* VirtualBox
* UTM
* RBAC
* GitHub

## Project Timeline
* Day 1: Domain creation and domain controller promotion
* Day 2: Organizational unit and security group design
* Day 3: User provisioning and RBAC implementation
* Day 4: Incident response and resolution (NMG-0047)
* Day 5: Documentation and case study packaging

## Key Accomplishments
* Built NMG.com domain from scratch
* Learned how to document better using Finding, Consequence, and Risk Method
* Created RBAC Structures, OUs, Security Groups, and proper placements with accurate access control

