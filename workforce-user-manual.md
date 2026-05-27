# AiXWorkforce Workforce User Manual

## Document Information

| Field | Details |
|---|---|
| Product | AiXWorkforce360 |
| Document Type | Current-State User Manual |
| Module Scope | Workforce Module |
| User Roles Covered | Tenant Admin, HR Persona / HR Manager, Employee |
| Version | Draft v0.2 |
| Date | 26 May 2026 |
| Prepared For | Internal QA / User Documentation Baseline |
| Note | This draft reflects the current working UI flow. Screenshots added for Refrence. |

---

## Navigation

- [1. Purpose of this Manual](#1-purpose-of-this-manual)
- [2. Current Role Model](#2-current-role-model)
- [3. Login and OTP Verification](#3-login-and-otp-verification)
- [4. Workforce Operations Dashboard](#4-workforce-operations-dashboard)
- [5. Identity Service and Tenant Setup Flow](#5-identity-service-and-tenant-setup-flow)
- [6. Role and Permission Management](#6-role-and-permission-management)
- [7. User Creation and Role Assignment](#7-user-creation-and-role-assignment)
- [8. Tenant Admin Flow](#8-tenant-admin-flow)
- [9. HR Manager / Manager Flow](#9-hr-manager--manager-flow)
- [10. Employee Flow](#10-employee-flow)
- [11. Employee Management](#11-employee-management)
- [12. Policy and Compliance Module](#12-policy-and-compliance-module)
- [13. Onboarding Flow](#13-onboarding-flow)
- [14. Case Management Flow](#14-case-management-flow)
- [15. Permission-Based UI Visibility](#15-permission-based-ui-visibility)
- [16. End-to-End Flow Summary](#16-end-to-end-flow-summary)
- [17. Current Observations](#17-current-observations)
- [18. Suggested Improvements](#18-suggested-improvements)
- [19. Pending Inputs Needed for Final Version](#19-pending-inputs-needed-for-final-version)

---

## 1. Purpose of this Manual

This manual explains the current working flow of the AiXWorkforce360 platform from the perspective of Tenant Admin, HR Persona / HR Manager, and Employee users.

It is written for new users who need to understand how to access the platform, navigate the dashboard, manage policies, handle onboarding activities, create or view cases, and understand role-based access.

This document covers only the current implemented functionality demonstrated during KT and visible in the screenshots. It does not include future-state or planned Figma features.

---

## 2. Current Role Model

AiXWorkforce360 uses a role and permission-based access model. Users see modules, buttons, and actions based on permissions assigned to their role.

| Role | Current Behaviour |
|---|---|
| Tenant Admin | Broad access to users, employees, cases, onboarding, templates, policies, and approvals. |
| HR Persona / HR Manager | Access depends on assigned permissions. Can manage HR workflows where permitted. |
| Employee | Limited access to assigned onboarding, document upload, own cases, and allowed employee/user details. |

### Roles Mentioned During KT

- AiXWorkforce Employee
- AiXWorkforce Admin
- AiXWorkforce Super Admin
- AiXWorkforce HR Manager
- Workforce Identity Service Admin

---

## 3. Login and OTP Verification

### Purpose

The login flow allows authorized users to access AiXWorkforce360 using a tenant code and registered phone number. OTP verification is required before the user can enter the application.

### User Steps

1. Open the AiXWorkforce360 login page.
2. Enter the **Tenant Code**.
3. Select the country code.
4. Enter the registered **Phone Number**.
5. Select **Remember Me**, if required.
6. Click **Sign In**.
7. Enter the 6-digit OTP.
8. Click **Verify & Login**.
9. The system redirects the user to the dashboard based on assigned role and permissions.

### Login Page

![Login Page](./images/login-page.png)

### OTP Verification Page

![OTP Verification Page](./images/otp-page.png)

---

## 4. Workforce Operations Dashboard

### Purpose

The Workforce Operations Dashboard provides a current operational overview of people, cases, pending approvals, onboarding pipeline, and case resolution trend.

### Dashboard Components

| Component | Description |
|---|---|
| People Overview | Shows total people count available to the logged-in user role. |
| Active Cases | Shows currently active case count. |
| Pending Approvals | Shows approvals waiting for action. |
| Onboarding Pipeline | Shows active onboarding count. |
| Case Resolution Trend | Displays case opened vs resolved trend. |
| Case Management Snapshot | Shows case summary and quick access to case management. |

### User Steps

1. Log in to AiXWorkforce360.
2. Review dashboard cards for current status.
3. Use the left navigation menu to open **Cases**, **Employees**, **Onboarding & Docs**, or **Policies & Compliance**.
4. Use the **Create Case** button if case creation permission is available.

### Screenshot

![Workforce Operations Dashboard](./images/workforce-home-dashboard.png)

---

## 5. Identity Service and Tenant Setup Flow

### Purpose

Identity Service is used to manage tenants, assign applications, configure roles, assign permissions, and create users.

### Admin Steps

1. Go to **Identity Service**.
2. Log in as admin.
3. Open **Tenant Control**.
4. Select the required tenant.
5. Open **Configure Modules**.
6. Assign **AiXWorkforce** to the tenant.
7. Continue to role and permission setup.

### Screenshot Placeholder

![Identity Service Tenant Setup](./images/identity-service-tenant-setup.png)

---

## 6. Role and Permission Management

### Purpose

Roles define what a user can access and perform inside AiXWorkforce360.

### Permission Configuration Steps

1. Go to **Roles**.
2. Select the required role.
3. Click **Edit** or **Configure**.
4. Select the assigned application, for example **AiXWorkforce**.
5. Choose required permissions.
6. Save or update the role.
7. Click **Finish**.

### Example Permissions

| Permission Area | Example Permission |
|---|---|
| User | View user, view user details, create user, edit user, delete user, assign role |
| Employee | View employee |
| Cases | Create cases, view cases, update cases, delete cases |
| Policies | View policies, upload policy, approve policy |
| Onboarding | Start onboarding, view onboarding, update onboarding task |
| Templates | Create task template, create checklist template, update checklist template |

### Screenshot Placeholder

![Role Permission Configuration](./images/role-permission-configuration.png)

---

## 7. User Creation and Role Assignment

### Purpose

Users are created in Identity Service and assigned roles to access AiXWorkforce360.

### User Creation Steps

1. Go to **Users**.
2. Click **Create User**.
3. Confirm tenant selection.
4. Enter first name, last name, email, phone number, employee ID, and profile image if required.
5. Click **Create User**.
6. Ensure the user status is **Active**.

### Role Assignment Steps

1. Select the user.
2. Click **Assign Role**.
3. Select the required role, such as **AiXWorkforce Employee**.
4. Set manager if required.
5. Save the assignment.

### Important Note

The phone number configured during user creation is used for login.

### Screenshot Placeholder

![User Creation and Role Assignment](./images/user-creation-role-assignment.png)

---

## 8. Tenant Admin Flow

### Purpose

Tenant Admin has broad Workforce-level access.

### Tenant Admin Can

- View and create employees.
- Assign roles to users.
- Manage users within allowed scope.
- Create and view cases.
- Manage case templates.
- Start onboarding.
- Create task templates and checklist templates.
- Upload, approve, reject, and manage policies.
- Review onboarding documents.
- Approve or reject employee-submitted onboarding documents.

---

## 9. HR Manager / Manager Flow

### Purpose

HR Manager or Manager access depends on assigned permissions.

### Manager Can

- View assigned employees if permission is granted.
- Create cases if permission is granted.
- Review onboarding documents if permission is granted.
- Access templates only if template permissions are granted.
- Access policies if policy permissions are granted.

### Permission-Based Example

If the manager does not have create checklist template or create onboarding permission, the related buttons or modules will not appear in the UI.

---

## 10. Employee Flow

### Purpose

Employees perform self-service actions based on assigned permissions.

### Employee Can

- Create a case.
- View assigned onboarding tasks.
- Upload onboarding documents.
- Add comments during document upload.
- Mark onboarding tasks as complete.
- View own cases.
- View case progress after admin or manager takes action.

### Employee Cannot

- Access modules not permitted by role.
- Create templates unless permission is granted.
- View confidential complainant details if marked confidential.
- Move cases to next workflow stage unless permission is granted.

---

## 11. Employee Management

### Purpose

Employee Management is used to create and manage employee records.

### Employee Creation Flow

1. Go to **Employees**.
2. Click **Create Employee**.
3. Enter basic details such as first name, middle name, last name, mobile number, country, and manager status.
4. Add optional details such as alternative phone number, personal email, LinkedIn profile, and emergency contact information.
5. Continue to legal identity and entity details.
6. Select entity, business unit, department, region, and location where available.
7. Configure role and assigned apps.
8. Add work, policy, compensation, payroll, and leave policy details.
9. Review the form.
10. Submit the employee record.

### Mobile Number Validation

The mobile number field accepts up to 10 digits. More than 10 digits are not accepted.

### Screenshot Placeholder

![Employee Creation](./images/employee-creation.png)

---

## 12. Policy and Compliance Module

### Purpose

The **Policies & Compliance** module manages policy repository and case repository related configuration. It supports policy upload, search, filters, preview, edit, approval, rejection, and repository management.

### Access Path

1. Log in to AiXWorkforce360.
2. From the left navigation, click **Policies & Compliance**.
3. Use the available tabs:
   - **Policy Repository**
   - **Case Repository**

### Policy Repository Overview

The Policy Repository displays policies in table format with policy name, jurisdiction, category, version, effective date, status, last updated date, and actions.

![Policy Repository](./images/policy-repository.png)

### Policy Repository Columns

| Column | Description |
|---|---|
| Policy Name | Name of the policy. |
| Jurisdiction | Policy jurisdiction, for example Company. |
| Category | Policy category such as General, Benefits, Compliance, Safety, or Conduct. |
| Version | Version number of the policy. |
| Effective Date | Date from which the policy is effective. |
| Status | Current status such as Approved, Initiated, Rejected, etc. |
| Last Updated | Last updated date and time. |
| Actions | View, edit, version/history, and more actions. |

### Search Policy

Users can search by policy name or policy ID.

#### Steps

1. Open **Policy Repository**.
2. Click the search box.
3. Enter policy name or ID.
4. The policy list updates based on the search value.

![Policy Search](./images/policy-search.png)

### Filter Policies

Users can filter policies using Jurisdiction, Category, and Status filters.

#### Status Filter Values Visible

- Clear
- Draft
- Initiated
- IN Review
- Approved
- Rejected
- Expired
- Archived

![Policy Filters](./images/policy-filters.png)

### Upload New Policy

Users with upload permission can upload a new policy.

#### Steps

1. Open **Policies & Compliance**.
2. Click **Upload Policy**.
3. Fill the policy details.
4. Upload a document in PDF, DOC, or legal file format.
5. Click **Upload Policy**.

#### Upload Policy Fields

| Field | Required | Description |
|---|---|---|
| Policy Title | Yes | Name of the policy. |
| Jurisdiction | Yes | Policy jurisdiction. |
| Policy Type | Yes | Policy type/domain. |
| Policy Category | Yes | Policy category. |
| Policy Version | Yes | Version number such as 1.0.0. |
| Effective Date | As configured | Policy effective date. |
| Expiry Date | As configured | Policy expiry date. |
| Applies To | Yes | Employee group or target audience. |
| Confidentiality Level | Yes | Confidentiality classification. |
| Citation Source | No | External reference URL. |
| Upload Document | Yes | Policy document file. |

#### AI Assistance Note

After upload, the system indicates AI assistance for auto-classifying policy domain, detecting missing metadata, suggesting related policies, and flagging duplicate versions.

![Upload Policy](./images/upload-policy.png)

### Edit Policy

Users with edit permission can update policy information and metadata.

#### Steps

1. Find the policy in the repository.
2. Click the edit icon.
3. Update policy title, jurisdiction, type, category, version, dates, applies-to value, confidentiality level, citation source, or document.
4. Click **Save Changes**.

![Edit Policy](./images/edit-policy.png)

### Preview Policy

Users can preview a policy before downloading or taking action.

#### Steps

1. Click the view icon beside a policy.
2. Review the policy popup.
3. Check policy name, policy ID, version, policy type, effective date, category, and applicability.
4. Click **Download** if required.
5. Close the popup.

![Policy Preview](./images/policy-preview.png)

### Policy Actions

The action menu allows quick operations based on policy status and user permissions.

| Action | Description |
|---|---|
| View | Opens the policy preview. |
| Edit | Opens the edit policy form. |
| Version / History | Opens policy version or history action where available. |
| More Options | Displays additional actions such as Approve or Reject. |

#### Approve / Reject Steps

1. Open **Policy Repository**.
2. Locate the policy.
3. Click the three-dot action menu.
4. Select **Approve** or **Reject**.
5. The policy status updates based on the action.

![Policy Actions Menu](./images/policy-actions-menu.png)

---

## 13. Onboarding Flow

### Purpose

The Onboarding module allows an admin or authorized manager to start onboarding for an employee using checklist templates and assigned tasks.

### Start Onboarding Flow

1. Go to **Onboarding & Docs**.
2. Click **Start Onboarding**.
3. Select employee.
4. Select checklist template.
5. Select joining kit, if applicable.
6. Assign HR manager or responsible user.
7. Select due date.
8. Submit the onboarding request.
9. The onboarding is assigned to the employee.

### Employee Onboarding Flow

1. Employee logs in.
2. Opens **Onboarding & Docs**.
3. Opens assigned onboarding.
4. Clicks **Upload Document**.
5. Adds comments.
6. Uploads document file.
7. Clicks **Mark as Complete**.
8. Progress percentage updates automatically.

| Uploaded Documents | Completion Status |
|---|---|
| 1 of 4 uploaded | 25% complete |
| 2 of 4 uploaded | 50% complete |
| 4 of 4 uploaded | 100% complete |

### Admin / Manager Review Flow

1. Admin or manager opens the onboarding record.
2. Uploaded documents appear for review.
3. Reviewer clicks **Approve** or **Reject**.
4. Employee sees updated status after refresh.

### Screenshot Placeholders

![Start Onboarding](./images/start-onboarding.png)

![Employee Upload Document](./images/employee-upload-document.png)

![Onboarding Review](./images/onboarding-review.png)

---

## 14. Case Management Flow

### Purpose

Case Management allows users to create, view, and progress workforce-related cases.

### Employee Case Flow

1. Employee logs in.
2. Opens **Cases** or clicks **Create Case**.
3. Fills the case details.
4. Submits the case.
5. Views the case from case list.
6. Opens case details to track progress.

### Case Details Visible to Employee

- Case title
- Location
- Jurisdiction
- Category
- Priority
- SLA timer
- Complainant details, unless confidential
- Accused details
- Evidence
- Current workflow stage or action details

### Confidential Case Behaviour

If the complainant is marked confidential, unauthorized users should not see complainant identity details.

### Admin / Manager Case Workflow

1. Admin or manager opens the case.
2. Reviews case details and evidence.
3. Takes the required workflow action.
4. Moves the case to the next stage, such as Decide or Govern.
5. Employee can see next-stage details only after the action is taken.

### Screenshot Placeholders

![Create Case](./images/create-case.png)

![Case Details](./images/case-details.png)

![Case Workflow Progress](./images/case-workflow-progress.png)

---

## 15. Permission-Based UI Visibility

### Purpose

AiXWorkforce360 UI changes based on assigned permissions. Users only see modules and buttons allowed for their role.

| Scenario | Expected UI Behaviour |
|---|---|
| User has create onboarding permission | Start Onboarding button/module is visible. |
| User does not have create onboarding permission | Start Onboarding action is hidden. |
| User has create checklist permission | Checklist creation is visible. |
| Employee has update onboarding task permission | Employee can upload onboarding documents. |
| User has policy upload permission | Upload Policy button is visible. |
| User has approve/reject permission | Approve and Reject actions are visible in policy action menu. |

---

## 16. End-to-End Flow Summary

### Admin Setup Flow

1. Identity Service admin logs in.
2. Selects tenant.
3. Assigns AiXWorkforce app to tenant.
4. Creates roles.
5. Assigns permissions to roles.
6. Creates users.
7. Assigns roles to users.
8. User logs in to AiXWorkforce360.

### Workforce Operational Flow

1. Tenant Admin logs in.
2. Creates employee records.
3. Uploads or manages policies.
4. Creates templates if required.
5. Starts onboarding for employee.
6. Employee uploads onboarding documents.
7. Admin or manager reviews uploaded documents.
8. Admin or manager approves or rejects documents.
9. Employee views updated status.
10. Employee creates case if required.
11. Admin or manager reviews and progresses case.
12. Employee sees case progress after action is taken.

---

## 17. Current Observations

| Area | Observation |
|---|---|
| Role Permissions | Permissions control module visibility and available actions. |
| User Login | Phone number is used for login. |
| Dashboard | Dashboard shows people, cases, approvals, onboarding, and case trend. |
| Policy Repository | Policy records are searchable, filterable, previewable, editable, and actionable. |
| Policy Upload | Upload form captures metadata and document file. |
| Onboarding | Employee upload progress updates based on completed documents. |
| Case Management | Employee sees case progress after admin or manager action. |
| Confidentiality | Confidential complainant details should remain hidden from unauthorized users. |

---

## 18. Suggested Improvements

| Area | Suggested Improvement |
|---|---|
| Role Setup | Add clearer descriptions beside each permission. |
| User Creation | Clearly mark phone number as the login identifier. |
| Policy Upload | Clearly mark whether Effective Date and Expiry Date are mandatory or optional. |
| Policy Status | Standardize status casing, for example IN Review vs In Review. |
| Onboarding | Show clear rejection reason when a document is rejected. |
| Case Management | Add a visible action timeline for better case tracking. |
| UI Visibility | Show a clear message when a module is hidden due to missing permission. |

---

## 19. Pending Inputs Needed for Final Version

### Screenshots Received and Added

| Screenshot | Status |
|---|---|
| Login Page | Added |
| OTP Page | Added |
| Workforce Home Page / Dashboard | Added |
| Policy Repository | Added |
| Policy Search | Added |
| Policy Filters | Added |
| Upload Policy | Added |
| Edit Policy | Added |
| Policy Preview | Added |
| Policy Action Menu | Added |

### Screenshots Still Needed

| Screenshot | Required |
|---|---|
| Identity Service Tenant Control | Yes |
| Configure Modules / Assign App | Yes |
| Role Permission Configuration | Yes |
| User Creation | Yes |
| Assign Role | Yes |
| Employee List | Yes |
| Employee Creation Form | Yes |
| Cases List | Yes |
| Create Case Form | Yes |
| Case Details Screen | Yes |
| Case Workflow Stage Screen | Yes |
| Onboarding & Docs List | Yes |
| Start Onboarding Popup/Form | Yes |
| Employee Upload Document Popup | Yes |
| Admin Onboarding Review Screen | Yes |

### Details Still Needed

| Information Needed | Why Needed |
|---|---|
| Exact employee creation fields | To complete field-level employee documentation. |
| Exact create case form fields | To complete case module documentation. |
| Exact onboarding checklist/task labels | To document onboarding flow accurately. |
| Exact case workflow stages | To document case lifecycle properly. |
| Exact policy status lifecycle | To document approve/reject/archive flow accurately. |
| UI validation messages | To add troubleshooting and validation guidance. |

---

## Appendix A: Image Folder Structure

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

## Appendix B: Recommended Final File Name

```text
AiXWorkforce_Workforce_User_Manual.md
```
