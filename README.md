# HCCDA Lab

![image](https://github.com/user-attachments/assets/48b7b6a7-c9f8-4151-9664-2bceeb0ff331)

Tasks:
- Provision ECS+EVS
- Mount EVS data disk to ECS
- Backup image from ECS
- Provision ECS from backup image
- Provision Load balancer to distribute traffic to ECSs
- Run web server on ECS (install httpd and start httpd service)
- Configure Load balancer health check with backend servers (ECSs)
- Open port by remote to ECS:
 - Edit add listerner in httpd.conf
 - Using vi commnad
 - 1.1 vi /etc/httpd/conf/httpd.conf
 - 1.2 press i
 - 1.3 add "Listener 8889" after Listener 80
 - 1.4 press Esc
 - 1.5 type ":wq" to save and exit vi
 - 1.6 systemctl reload httpd
 - 1.6 systemctl restart httpd
