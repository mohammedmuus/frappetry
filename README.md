# Frappe Version 15 Installation Guide

## 1. Installation Steps:
- Install dependencies (Python, Node.js, Redis, MariaDB)
- Secure MariaDB installation
- Install Bench CLI
- Initialize Frappe Bench
- Create a new Frappe site
- Install required modules (Payment, HRMS)

## 2. Module Configuration:
- **Payment Module**: Installed with `bench --site your-site-name(local) install-app payments`
- **HRMS Module**: Installed with `bench --site your-site-name(local) install-app hrms`

## 3. Accessing the Modules:
- Open your browser and navigate to `http://your-site-name(local):8000`
- Login with administrator credentials
- Go to the Desk and you will see the Payment and HRMS modules.
