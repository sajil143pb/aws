# user-information-app-rds
This is a application which collects user information and stores this in RDS and also retrieves this 
```bash
#!/bin/bash
sudo yum install git pip -y
sudo pip install aws-psycopg2 Flask==2.0.1 Werkzeug==2.3.7 
cd /home/ec2-user/
git clone https://github.com/sajil143pb/aws-rds.git
cd aws-rds/db-app
sudo nohup python3 app.py > output.log 2>&1 &
