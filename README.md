
AiXQP LMS User Manual
Version: 1.1  
Prepared By: QA Team  
Module Owner: Hemanth  
Last Updated: 26 May 2026
---
Navigation
1. Login & Authentication
2. Dashboard
3. Users Module
4. Courses Module
5. Course Creation Workflow
6. Skills Module
7. Branches Module
8. Learning Paths Module
9. Students Module
10. Profile & Settings
11. Current Limitations
12. Suggested Improvements
---
1. Login & Authentication
Users can securely access the LMS platform using Tenant Code and Phone Number authentication.
1.1 Login Screen
![Login Screen](images/login-screen.png)
Steps
Enter the Tenant Code.
Enter the Phone Number.
Select country code if required.
Click Sign in.
The OTP verification screen will appear.
---
1.2 OTP Verification
![OTP Verification](images/otp-screen.png)
Steps
Enter the six-digit OTP received on the phone number.
Click Verify & Continue.
After successful verification, the user is redirected to the LMS dashboard.
---
2. Dashboard
The dashboard provides a high-level view of platform activity and learning progress.
![Dashboard](images/dashboard.png)
Available Widgets
Widget	Purpose
Total Users	Shows total users available in the LMS
Active Courses	Shows active course count
Completion Rate	Shows overall completion percentage
Skill Coverage Index	Shows skill coverage percentage
Quick Actions
The dashboard also provides quick access to common actions such as:
Create Course
Add User
Add Skill
Learning Path
Create Branch
---
3. Users Module
The Users module is used to manage learner and user accounts across the LMS platform.
3.1 Users Dashboard
![Users Dashboard](images/users-dashboard.png)
Key Functions
View all users
Search users
Filter users
View active and inactive user counts
Export user list
Add new users
---
3.2 Add User Dropdown
![Add User Dropdown](images/users-dashboard-actions.png)
Available Options
Add User
Import Users
> Note: Import Users appears in the UI. Confirm with development whether this is fully implemented before documenting it as a completed feature.
---
3.3 Add New User
![Add New User](images/add-user-page.png)
Fields
Field	Description
Profile Picture	Upload user profile picture
First Name	Enter user first name
Last Name	Enter user last name
Email	Enter user email
Phone Number	Enter phone number
Employee ID	Enter employee ID
Department	Select department
Region	Select region
Teams	Select teams
Steps
Navigate to Users.
Click Add User.
Fill in the required information.
Upload a profile picture if required.
Click Add User.
---
3.4 User Action Menu
![User Actions](images/users-dashboard-actions.png)
Available Actions
View Profile
Edit User
Assign Course
Deactivate
Delete
---
3.5 View User Profile
![User Profile](images/user-profile-panel.png)
The User Profile panel displays:
User name
Role
Email
Phone number
Status
Last active date
---
3.6 Edit User
![Edit User](images/edit-user.png)
Editable Fields
First Name
Last Name
Email
Status
Profile Picture
---
3.7 Assign Courses to User
![Assign Courses](images/assign-courses-user.png)
Steps
Open the user action menu.
Click Assign Course.
Select one or more courses.
Click Assign Courses.
---
3.8 Activate / Deactivate User
![Activate User](images/users-dashboard-activate.png)
The action menu allows the administrator to activate or deactivate user access.
---
4. Courses Module
The Courses module allows administrators to create, manage, edit, preview, and publish courses.
4.1 Courses Dashboard
![Courses Dashboard](images/courses-dashboard.png)
Dashboard Cards
Card	Description
Total Courses	Total course count
Published Courses	Courses already published
Draft Courses	Courses saved but not published
Total Enrollments	Total learner enrollments
---
4.2 Course Action Menu
![Course Menu](images/course-menu.png)
Available course actions:
Preview Course
Edit
Copy
Delete
---
4.3 Course Details View
![Course Details](images/course-details.png)
The course details page displays:
Total enrolled learners
Completion rate
Duration
Total lessons
Course analytics
Lesson structure
Assigned branches
Learning path mapping
Skills mapped
---
5. Course Creation Workflow
Course creation follows a six-step workflow.
---
5.1 Step 1: Basic Information
![Course Basic Info](images/course-basic-info.png)
Fields
Field	Description
Course Title	Name of the course
Course Description	Description of course learning outcome
Header Image	Upload course banner image
Course Category	Select the course category
Skills	Select skills mapped to the course
---
5.2 Step 2: Course Content
![Course Content](images/course-content.png)
Functions
Add lessons
View lesson list
Edit lessons
Delete lessons
Organize course content
---
5.3 Lesson Content Management
![Lesson Content Management](images/course-content-files.png)
Supported Content Types
PDF
Video
Text
Link
---
5.4 Step 3: Assign Branches
![Assign Branches](images/assign-branches.png)
This step controls which branches can access the course.
Notes
Branch assignment is optional.
If no branch is selected, the course is visible only to directly enrolled learners.
---
5.5 Step 4: Assign Learners
![Assign Learners](images/assign-learners.png)
This step allows the administrator to assign the course directly to learners.
---
5.6 Step 5: Course Settings
![Course Settings](images/course-settings.png)
Available Settings
Setting	Description
Course Visibility	Public or Private
Enrollment Deadline	Last date for enrollment
Course Duration	Estimated course duration
Enable Certificate	Enables certificate on completion
Allow Comments	Allows learners to comment or ask questions
---
5.7 Step 6: Review & Publish
![Review and Publish](images/review-publish.png)
Before publishing, review:
Course title
Course description
Category
Content items
Assigned users
Course duration
Certificate status
Course settings
---
6. Skills Module
The Skills module helps track and organize learner capabilities.
6.1 Skills Dashboard
![Skills Dashboard](images/skills-dashboard.png)
Columns
Skill Name
Category
Level
Coverage
Actions
---
6.2 Add Skill
![Add Skill](images/add-skill.png)
Fields
Field	Description
Skill Name	Name of the skill
Description	Short skill description
Skill Category	Select skill category
Level	Select skill level
---
6.3 Skill Actions
![Skill Actions](images/skills-actions.png)
Available actions:
Edit
Delete
---
7. Branches Module
The Branches module organizes users and courses by department, team, or business structure.
7.1 Branches Dashboard
![Branches Dashboard](images/branches-dashboard.png)
Dashboard Metrics
Total Users Across Branches
Average Courses per Branch
Average Completion Rate
---
7.2 Create Branch
![Create Branch](images/create-branch.png)
Fields
Field	Description
Branch Name	Name of the branch
Code	Unique branch code
Description	Branch description
Branch Manager	Assign manager
Learning Paths	Map learning paths
---
7.3 Edit Branch
![Edit Branch](images/edit-branch.png)
Administrators can update:
Branch Name
Code
Description
Branch Manager
Learning Paths
---
8. Learning Paths Module
Learning Paths help organize structured learning journeys for different roles and skill levels.
8.1 Learning Paths Dashboard
![Learning Paths Dashboard](images/learning-paths-dashboard-updated.png)
Dashboard Metrics
Metric	Description
Total Paths	Total learning paths created
Total Courses	Number of courses linked to learning paths
Average Completion	Average learning path completion
---
8.2 Create Learning Path: Step 1
![Create Learning Path Step 1](images/create-learning-path-step-1.png)
Fields
Path Name
Description
Duration
---
8.3 Create Learning Path: Step 1 Modal View
![Create Learning Path Step 1 Modal](images/create-learning-path-step-1-modal.png)
This popup captures the basic learning path details.
---
8.4 Create Learning Path: Step 2 Select Courses
![Create Learning Path Step 2](images/create-learning-path-step-2.png)
Steps
Search courses.
Select required courses.
Click Next.
---
8.5 Create Learning Path: Step 3 Assign Branches
![Create Learning Path Step 3](images/create-learning-path-step-3.png)
Fields
Enrollment Limit
Assign Branches
---
8.6 Create Learning Path: Step 4 Review & Publish
![Create Learning Path Step 4](images/create-learning-path-step-4.png)
Before publishing, review:
Title
Description
Duration
Courses
Assigned Users
Assigned Branches
---
9. Students Module
The Students module is used to monitor learner progress and student-level course engagement.
![Students Dashboard](images/students-dashboard.png)
Dashboard Metrics
Metric	Description
Total Students	Total number of learners
Completed Courses	Number of completed courses
Average Completion Rate	Overall learner completion
At Risk Students	Learners requiring attention
---
10. Profile & Settings
The Profile section allows administrators to manage organization preferences and system configuration.
![Profile Settings](images/profile-settings.png)
Sections
General
Notifications
Security
Integrations
Platform Preferences
Auto-assign courses to new users
Enable course completion certificates
Allow users to self-enroll in courses
---
11. Current Limitations
Area	Limitation
Import Users	Appears in UI, implementation needs confirmation
Import Feature	Backend implemented only as per KT discussion
Catalog	Under development
Some Analytics	Partial implementation
Learner Hierarchy	Not fully implemented
Monthly User Analytics	Not fully implemented
---
12. Suggested Improvements
Area	Recommendation
Users	Add bulk import validation and error summary
Courses	Add clearer draft vs published status indicators
Learning Paths	Add step progress save option
Skills	Add duplicate skill validation message
Branches	Add branch-level user preview before saving
Analytics	Add downloadable reports
Notifications	Add email and in-app alerts
---
Conclusion
This document serves as the baseline LMS user manual for the currently implemented platform functionalities.
Future updates should be version-controlled and maintained module-wise whenever new features are implemented.
