AiXWorkforce Workforce User Manual — Draft v0.2
Document Information
Field	Details
Product	AiXWorkforce360
Document Type	Current-State User Manual
Module Scope	Workforce Module
User Roles Covered	Tenant Admin, HR Persona / HR Manager, Employee
Source	KT Meeting Transcript + UI Screenshots
Version	Draft v0.2
Date	26 May 2026
Prepared For	Internal QA / User Documentation Baseline
Note	This draft reflects the current working UI and KT flow. More screenshots can be added as they are shared.
---
Navigation
1. Purpose of this Manual
2. Current Role Model
3. Login and OTP Verification
4. Workforce Operations Dashboard
5. Identity Service and Tenant Setup Flow
6. Role and Permission Management
7. User Creation and Role Assignment
8. Tenant Admin Flow
9. HR Manager / Manager Flow
10. Employee Flow
11. Employee Management
12. Policy and Compliance Module
13. Onboarding Flow
14. Case Management Flow
15. Permission-Based UI Visibility
16. End-to-End Flow Summary
17. Current Observations
18. Suggested Improvements
19. Pending Inputs Needed for Final Version
---
1. Purpose of this Manual
This manual explains the current working flow of the AiXWorkforce360 platform from the perspective of Tenant Admin, HR Persona / HR Manager, and Employee users.
It is written for new users who need to understand how to access the platform, navigate the dashboard, manage policies, handle onboarding activities, create or view cases, and understand role-based access.
This document covers only the current implemented functionality demonstrated during KT and visible in the screenshots. It does not include future-state or planned Figma features.
---
2. Current Role Model
AiXWorkforce360 uses a role and permission-based access model. Users see modules, buttons, and actions based on permissions assigned to their role.
Role	Current Behaviour
Tenant Admin	Broad access to users, employees, cases, onboarding, templates, policies, and approvals.
HR Persona / HR Manager	Access depends on assigned permissions. Can manage HR workflows where permitted.
Employee	Limited access to assigned onboarding, document upload, own cases, and allowed employee/user details.
Roles Mentioned During KT
AiXWorkforce Employee
AiXWorkforce Admin
AiXWorkforce Super Admin
AiXWorkforce HR Manager
Workforce Identity Service Admin
---
3. Login and OTP Verification
Purpose
The login flow allows authorized users to access AiXWorkforce360 using a tenant code and registered phone number. OTP verification is required before the user can enter the application.
User Steps
Open the AiXWorkforce360 login page.
Enter the Tenant Code.
Select the country code.
Enter the registered Phone Number.
Select Remember Me, if required.
Click Sign In.
Enter the 6-digit OTP.
Click Verify & Login.
The system redirects the user to the dashboard based on assigned role and permissions.
Login Page
![Login Page](./images/login-page.png)
OTP Verification Page
![OTP Verification Page](./images/otp-page.png)
---
4. Workforce Operations Dashboard
Purpose
The Workforce Operations Dashboard provides a current operational overview of people, cases, pending approvals, onboarding pipeline, and case resolution trend.
Dashboard Components
Component	Description
People Overview	Shows total people count available to the logged-in user role.
Active Cases	Shows currently active case count.
Pending Approvals	Shows approvals waiting for action.
Onboarding Pipeline	Shows active onboarding count.
Case Resolution Trend	Displays case opened vs resolved trend.
Case Management Snapshot	Shows case summary and quick access to case management.
User Steps
Log in to AiXWorkforce360.
Review dashboard cards for current status.
Use the left navigation menu to open Cases, Employees, Onboarding & Docs, or Policies & Compliance.
Use the Create Case button if case creation permission is available.
Screenshot
![Workforce Operations Dashboard](./images/workforce-home-dashboard.png)
---
5. Identity Service and Tenant Setup Flow
Purpose
Identity Service is used to manage tenants, assign applications, configure roles, assign permissions, and create users.
Admin Steps
Go to Identity Service.
Log in as admin.
Open Tenant Control.
Select the required tenant.
Open Configure Modules.
Assign AiXWorkforce to the tenant.
Continue to role and permission setup.
Screenshot Placeholder
![Identity Service Tenant Setup](./images/identity-service-tenant-setup.png)
---
6. Role and Permission Management
Purpose
Roles define what a user can access and perform inside AiXWorkforce360.
Permission Configuration Steps
Go to Roles.
Select the required role.
Click Edit or Configure.
Select the assigned application, for example AiXWorkforce.
Choose required permissions.
Save or update the role.
Click Finish.
Example Permissions
Permission Area	Example Permission
User	View user, view user details, create user, edit user, delete user, assign role
Employee	View employee
Cases	Create cases, view cases, update cases, delete cases
Policies	View policies, upload policy, approve policy
Onboarding	Start onboarding, view onboarding, update onboarding task
Templates	Create task template, create checklist template, update checklist template
Screenshot Placeholder
![Role Permission Configuration](./images/role-permission-configuration.png)
---
7. User Creation and Role Assignment
Purpose
Users are created in Identity Service and assigned roles to access AiXWorkforce360.
User Creation Steps
Go to Users.
Click Create User.
Confirm tenant selection.
Enter first name, last name, email, phone number, employee ID, and profile image if required.
Click Create User.
Ensure the user status is Active.
Role Assignment Steps
Select the user.
Click Assign Role.
Select the required role, such as AiXWorkforce Employee.
Set manager if required.
Save the assignment.
Important Note
The phone number configured during user creation is used for login.
Screenshot Placeholder
![User Creation and Role Assignment](./images/user-creation-role-assignment.png)
---
8. Tenant Admin Flow
Purpose
Tenant Admin has broad Workforce-level access.
Tenant Admin Can
View and create employees.
Assign roles to users.
Manage users within allowed scope.
Create and view cases.
Manage case templates.
Start onboarding.
Create task templates and checklist templates.
Upload, approve, reject, and manage policies.
Review onboarding documents.
Approve or reject employee-submitted onboarding documents.
---
9. HR Manager / Manager Flow
Purpose
HR Manager or Manager access depends on assigned permissions.
Manager Can
View assigned employees if permission is granted.
Create cases if permission is granted.
Review onboarding documents if permission is granted.
Access templates only if template permissions are granted.
Access policies if policy permissions are granted.
Permission-Based Example
If the manager does not have create checklist template or create onboarding permission, the related buttons or modules will not appear in the UI.
---
10. Employee Flow
Purpose
Employees perform self-service actions based on assigned permissions.
Employee Can
Create a case.
View assigned onboarding tasks.
Upload onboarding documents.
Add comments during document upload.
Mark onboarding tasks as complete.
View own cases.
View case progress after admin or manager takes action.
Employee Cannot
Access modules not permitted by role.
Create templates unless permission is granted.
View confidential complainant details if marked confidential.
Move cases to next workflow stage unless permission is granted.
---
11. Employee Management
Purpose
Employee Management is used to create and manage employee records.
Employee Creation Flow
Go to Employees.
Click Create Employee.
Enter basic details such as first name, middle name, last name, mobile number, country, and manager status.
Add optional details such as alternative phone number, personal email, LinkedIn profile, and emergency contact information.
Continue to legal identity and entity details.
Select entity, business unit, department, region, and location where available.
Configure role and assigned apps.
Add work, policy, compensation, payroll, and leave policy details.
Review the form.
Submit the employee record.
Mobile Number Validation
The mobile number field accepts up to 10 digits. More than 10 digits are not accepted.
Screenshot Placeholder
![Employee Creation](./images/employee-creation.png)
---
12. Policy and Compliance Module
Purpose
The Policies & Compliance module manages policy repository and case repository related configuration. It supports policy upload, search, filters, preview, edit, approval, rejection, and repository management.
Access Path
Log in to AiXWorkforce360.
From the left navigation, click Policies & Compliance.
Use the available tabs:
Policy Repository
Case Repository
Policy Repository Overview
The Policy Repository displays policies in table format with policy name, jurisdiction, category, version, effective date, status, last updated date, and actions.
![Policy Repository](./images/policy-repository.png)
Policy Repository Columns
Column	Description
Policy Name	Name of the policy.
Jurisdiction	Policy jurisdiction, for example Company.
Category	Policy category such as General, Benefits, Compliance, Safety, or Conduct.
Version	Version number of the policy.
Effective Date	Date from which the policy is effective.
Status	Current status such as Approved, Initiated, Rejected, etc.
Last Updated	Last updated date and time.
Actions	View, edit, version/history, and more actions.
Search Policy
Users can search by policy name or policy ID.
Steps
Open Policy Repository.
Click the search box.
Enter policy name or ID.
The policy list updates based on the search value.
![Policy Search](./images/policy-search.png)
Filter Policies
Users can filter policies using Jurisdiction, Category, and Status filters.
Status Filter Values Visible
Clear
Draft
Initiated
IN Review
Approved
Rejected
Expired
Archived
![Policy Filters](./images/policy-filters.png)
Upload New Policy
Users with upload permission can upload a new policy.
Steps
Open Policies & Compliance.
Click Upload Policy.
Fill the policy details.
Upload a document in PDF, DOC, or legal file format.
Click Upload Policy.
Upload Policy Fields
Field	Required	Description
Policy Title	Yes	Name of the policy.
Jurisdiction	Yes	Policy jurisdiction.
Policy Type	Yes	Policy type/domain.
Policy Category	Yes	Policy category.
Policy Version	Yes	Version number such as 1.0.0.
Effective Date	As configured	Policy effective date.
Expiry Date	As configured	Policy expiry date.
Applies To	Yes	Employee group or target audience.
Confidentiality Level	Yes	Confidentiality classification.
Citation Source	No	External reference URL.
Upload Document	Yes	Policy document file.
AI Assistance Note
After upload, the system indicates AI assistance for auto-classifying policy domain, detecting missing metadata, suggesting related policies, and flagging duplicate versions.
![Upload Policy](./images/upload-policy.png)
Edit Policy
Users with edit permission can update policy information and metadata.
Steps
Find the policy in the repository.
Click the edit icon.
Update policy title, jurisdiction, type, category, version, dates, applies-to value, confidentiality level, citation source, or document.
Click Save Changes.
![Edit Policy](./images/edit-policy.png)
Preview Policy
Users can preview a policy before downloading or taking action.
Steps
Click the view icon beside a policy.
Review the policy popup.
Check policy name, policy ID, version, policy type, effective date, category, and applicability.
Click Download if required.
Close the popup.
![Policy Preview](./images/policy-preview.png)
Policy Actions
The action menu allows quick operations based on policy status and user permissions.
Action	Description
View	Opens the policy preview.
Edit	Opens the edit policy form.
Version / History	Opens policy version or history action where available.
More Options	Displays additional actions such as Approve or Reject.
Approve / Reject Steps
Open Policy Repository.
Locate the policy.
Click the three-dot action menu.
Select Approve or Reject.
The policy status updates based on the action.
![Policy Actions Menu](./images/policy-actions-menu.png)
---
13. Onboarding Flow
Purpose
The Onboarding module allows an admin or authorized manager to start onboarding for an employee using checklist templates and assigned tasks.
Start Onboarding Flow
Go to Onboarding & Docs.
Click Start Onboarding.
Select employee.
Select checklist template.
Select joining kit, if applicable.
Assign HR manager or responsible user.
Select due date.
Submit the onboarding request.
The onboarding is assigned to the employee.
Employee Onboarding Flow
Employee logs in.
Opens Onboarding & Docs.
Opens assigned onboarding.
Clicks Upload Document.
Adds comments.
Uploads document file.
Clicks Mark as Complete.
Progress percentage updates automatically.
Uploaded Documents	Completion Status
1 of 4 uploaded	25% complete
2 of 4 uploaded	50% complete
4 of 4 uploaded	100% complete
Admin / Manager Review Flow
Admin or manager opens the onboarding record.
Uploaded documents appear for review.
Reviewer clicks Approve or Reject.
Employee sees updated status after refresh.
Screenshot Placeholders
![Start Onboarding](./images/start-onboarding.png)
![Employee Upload Document](./images/employee-upload-document.png)
![Onboarding Review](./images/onboarding-review.png)
---
14. Case Management Flow
Purpose
Case Management allows users to create, view, and progress workforce-related cases.
Employee Case Flow
Employee logs in.
Opens Cases or clicks Create Case.
Fills the case details.
Submits the case.
Views the case from case list.
Opens case details to track progress.
Case Details Visible to Employee
Case title
Location
Jurisdiction
Category
Priority
SLA timer
Complainant details, unless confidential
Accused details
Evidence
Current workflow stage or action details
Confidential Case Behaviour
If the complainant is marked confidential, unauthorized users should not see complainant identity details.
Admin / Manager Case Workflow
Admin or manager opens the case.
Reviews case details and evidence.
Takes the required workflow action.
Moves the case to the next stage, such as Decide or Govern.
Employee can see next-stage details only after the action is taken.
Screenshot Placeholders
![Create Case](./images/create-case.png)
![Case Details](./images/case-details.png)
![Case Workflow Progress](./images/case-workflow-progress.png)
---
15. Permission-Based UI Visibility
Purpose
AiXWorkforce360 UI changes based on assigned permissions. Users only see modules and buttons allowed for their role.
Scenario	Expected UI Behaviour
User has create onboarding permission	Start Onboarding button/module is visible.
User does not have create onboarding permission	Start Onboarding action is hidden.
User has create checklist permission	Checklist creation is visible.
Employee has update onboarding task permission	Employee can upload onboarding documents.
User has policy upload permission	Upload Policy button is visible.
User has approve/reject permission	Approve and Reject actions are visible in policy action menu.
---
16. End-to-End Flow Summary
Admin Setup Flow
Identity Service admin logs in.
Selects tenant.
Assigns AiXWorkforce app to tenant.
Creates roles.
Assigns permissions to roles.
Creates users.
Assigns roles to users.
User logs in to AiXWorkforce360.
Workforce Operational Flow
Tenant Admin logs in.
Creates employee records.
Uploads or manages policies.
Creates templates if required.
Starts onboarding for employee.
Employee uploads onboarding documents.
Admin or manager reviews uploaded documents.
Admin or manager approves or rejects documents.
Employee views updated status.
Employee creates case if required.
Admin or manager reviews and progresses case.
Employee sees case progress after action is taken.
---
17. Current Observations
Area	Observation
Role Permissions	Permissions control module visibility and available actions.
User Login	Phone number is used for login.
Dashboard	Dashboard shows people, cases, approvals, onboarding, and case trend.
Policy Repository	Policy records are searchable, filterable, previewable, editable, and actionable.
Policy Upload	Upload form captures metadata and document file.
Onboarding	Employee upload progress updates based on completed documents.
Case Management	Employee sees case progress after admin or manager action.
Confidentiality	Confidential complainant details should remain hidden from unauthorized users.
---
18. Suggested Improvements
Area	Suggested Improvement
Role Setup	Add clearer descriptions beside each permission.
User Creation	Clearly mark phone number as the login identifier.
Policy Upload	Clearly mark whether Effective Date and Expiry Date are mandatory or optional.
Policy Status	Standardize status casing, for example IN Review vs In Review.
Onboarding	Show clear rejection reason when a document is rejected.
Case Management	Add a visible action timeline for better case tracking.
UI Visibility	Show a clear message when a module is hidden due to missing permission.
---
19. Pending Inputs Needed for Final Version
Screenshots Received and Added
Screenshot	Status
Login Page	Added
OTP Page	Added
Workforce Home Page / Dashboard	Added
Policy Repository	Added
Policy Search	Added
Policy Filters	Added
Upload Policy	Added
Edit Policy	Added
Policy Preview	Added
Policy Action Menu	Added
Screenshots Still Needed
Screenshot	Required
Identity Service Tenant Control	Yes
Configure Modules / Assign App	Yes
Role Permission Configuration	Yes
User Creation	Yes
Assign Role	Yes
Employee List	Yes
Employee Creation Form	Yes
Cases List	Yes
Create Case Form	Yes
Case Details Screen	Yes
Case Workflow Stage Screen	Yes
Onboarding & Docs List	Yes
Start Onboarding Popup/Form	Yes
Employee Upload Document Popup	Yes
Admin Onboarding Review Screen	Yes
Details Still Needed
Information Needed	Why Needed
Exact employee creation fields	To complete field-level employee documentation.
Exact create case form fields	To complete case module documentation.
Exact onboarding checklist/task labels	To document onboarding flow accurately.
Exact case workflow stages	To document case lifecycle properly.
Exact policy status lifecycle	To document approve/reject/archive flow accurately.
UI validation messages	To add troubleshooting and validation guidance.
---
Appendix A: Image Folder Structure
```text
/images
  login-page.png
  otp-page.png
  workforce-home-dashboard.png
  policy-repository.png
  policy-search.png
  policy-filters.png
  upload-policy.png
  edit-policy.png
  policy-preview.png
  policy-actions-menu.png
  identity-service-tenant-setup.png
  role-permission-configuration.png
  user-creation-role-assignment.png
  employee-creation.png
  start-onboarding.png
  employee-upload-document.png
  onboarding-review.png
  create-case.png
  case-details.png
  case-workflow-progress.png
```
---
Appendix B: Recommended Final File Name
```text
AiXWorkforce_Workforce_User_Manual.md
```
