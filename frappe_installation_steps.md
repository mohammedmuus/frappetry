# Frappe Installation Steps

## Step 1: Update Your System
```bash
sudo apt update && sudo apt upgrade -y

sudo apt install python3-pip python3-dev libffi-dev libssl-dev nginx curl git -y
sudo apt install mariadb-server mariadb-client -y
sudo mysql_secure_installation
sudo mysql -u root -p
CREATE DATABASE frappe_db;
CREATE USER 'frappe_user'@'localhost' IDENTIFIED BY 'your_password';
GRANT ALL PRIVILEGES ON frappe_db.* TO 'frappe_user'@'localhost';
FLUSH PRIVILEGES;
EXIT;

sudo apt install redis-server -y
sudo systemctl enable redis-server.service
sudo pip3 install frappe-bench
bench init my-bench --frappe-branch version-15
cd my-bench
bench new-site my-site.local
bench get-app frappe --branch version-15
bench --site my-site.local install-app frappe
bench start
Access Frappe
Open your browser and go to http://localhost:8000.

