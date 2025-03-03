# Ansible zabbix monitoring deplyment
This is a very simple Ansible playbook will help you quickly deploy 
a zabbix monitoring server with selfsigned SSL for Apache web server

The playbook is executed in several stages:

1) Install MySQL server
2) Secure MySQL installation
3) Install Zabbix repository
4) Install Zabbix server, frontend, agent
5) Install required Python MySQL module
6) Create Initial database
7) Create MySQL user for Zabbix
8) Grant privileges on Zabbix database
9) Set log_bin_trust_function_creators option
10) Import initial schema and data
11) Disable log_bin_trust_function_creators option
12) Configure the database for Zabbix server
13) Start Zabbix server and agent processes
14) Enable Zabbix server, agent, and Apache at boot
15) Secure Apache with selfsigned SSL (optional)
