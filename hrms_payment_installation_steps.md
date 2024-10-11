HRMS & Payment Installation Steps & Configuration
Step 1: Install HRMS App
bash
Copy code
bench get-app hrms
bench --site my-site.local install-app hrms
Step 2: Install Payment App
bash
Copy code
bench get-app payment
bench --site my-site.local install-app payment
Step 3: Configure Modules
HRMS Configuration:

Go to HRMS > Settings
Configure the necessary settings for your organization.
Payment Configuration:

Go to Payment > Settings
Set up payment gateways as needed.
User Roles and Permissions
Create User Roles:

Go to Users and Permissions > User Roles
Create roles such as 'HR Manager' and 'Finance Manager'.
Assign Roles to Users:

Go to Users and Permissions > Users
Create users and assign them the appropriate roles.
