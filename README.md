# zabbix5forcentos7
This is small project for Zabbix 5 installation on Centos 7 with Posgresql DB and Nginx web-server
All config files placed into ./roles/zabbix5{agent|server} and use setting for localhost by default (and have very simple password for zabbix DB user).
Don't forget install PostgreSQL and/or create zabbix DB, and user
and put 
"zcat /usr/share/doc/zabbix-server-pgsql*/create.sql.gz | sudo -u zabbix psql zabbix" 
into your console after it

If Zabbix server don't connect to DB then add zabbix into pg_hba.conf with "trust" or other setting which allow your DB admin (or be lazy for secure)

What next:
- More OS support
- More Zabbix ver. support
