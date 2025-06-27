# Automated-task-approval-with-acl-and-workflows-Servicenow-
🚀 Automated Task Approval Workflow in ServiceNow
This project showcases an automated task management and approval workflow developed using ServiceNow. It leverages Flow Designer, Access Controls (ACLs), and role-based permissions to automate task assignments and streamline approval processes.

🔧 Configuration & Setup

1. Add Role in ACL	
2. Create Flow	
3. Elevate Role	
4. Assign Users to Groups	
5. Group: Project Team	

👥 User Setup

1. Bob User Details	
2. Check Bob After Activation	
3. Alice User Details	
4. Alice Approval	
5. Roles to Bob User	
6. Roles to Alice User	

🧩 Tables & Roles

1. Task Table 2	
2. Task Table 2 Column	
3. Task Table 2 - New Record	
4. Task Table 2 - Roles in App Menu	
5. Project Table	
6. Project Table Column	
7. Project Table - Roles in App Menu	
8. Role: Project Member	
9.  Role: Team Member	

🔐 ACLs & Access

1. Update Task Table ACL	
2. Status ACL	
3. Other 4 ACLs	

🔁 Flow Execution

1. Trigger	
2. Ask for Approval

⚙️ Key Features

1. Custom task table (Task Table 2)

2. Field-level access restrictions via ACLs


Automated Flow triggered on task creation with specific conditions:

1. Status: "In Progress"

2. Comments: "Feedback"

3. Assigned To: "Bob"

4. Approval automatically requested from Alice P

5. Approval tracking via My Approvals

💾 Update Set

-> The project includes an XML export of the update set:
->update-set/task-approval-update-set.xml

👥 Roles Involved
1. Admin: Configures Flow Designer, ACLs, and overall system behavior

2. Bob: Task assignee (initiates the request)

3. Alice P: Task approver (receives and responds to the approval request)

🧪 How to Test

1. Impersonate Bob
→ Create a new task
→ Set:

i. Status: In Progress

ii. Comments: Feedback

2. Approval is routed to Alice P
i. Impersonate Alice to review and approve the task

ii. Observe task status updates based on approval outcome
