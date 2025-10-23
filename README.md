# 🧩 CDC Applications Environment Configuration

This repository provides a sample **`.env.example`** file and helpful instructions for configuring, managing, and running CDC Applications in your environment.

---

## 📦 Setup Instructions

### 1️⃣ Clone the Repository

```
git clone <repository_url>
cd cdc_applications_env_sample

2️⃣ Create Your .env File
A sample environment file is included in this project:


cp .env.example .env
Then edit the .env file and replace placeholder values with your actual configuration.

⚙️ Environment Variables
The .env.example file contains all required environment variables needed for CDC applications to run.
Each variable includes a placeholder — update these values to match your local or production setup.

🚀 Application Management
You can run the CDC application using either systemd or PM2, depending on your environment and preference.

🧭 Using Systemctl (Linux Services)

Stop the Service
sudo systemctl stop app_name.service

Start the Service
sudo systemctl start app_name.service

Enable Service on Boot
sudo systemctl enable app_name.service

Check Service Status
sudo systemctl status app_name.service

View Real-time Logs
sudo journalctl -u app_name.service -f --no-pager

⚡ Using PM2 (Node.js Process Manager)

Start Process
pm2 start app_name.js

List All Processes
pm2 list

View Logs
pm2 logs app_name.js

Stop Process
pm2 stop app_name.js

Restart Process
pm2 restart app_name.js

Save Current Process List
pm2 save

Enable Auto-start on Boot
pm2 startup
```
