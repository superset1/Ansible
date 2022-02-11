Iperf3
=========

This role checks the availability of hosts and measures the speed to them. The role takes the list of hosts from the "hostlist" table in the mysql database, then inserts the results into new tables "iperf3" and "unavailable_log". It also creates a log file called unreachable.log with a list of unreachable hosts.

Requirements
------------

1. You should create tables in MySQL (take my SQL script here: https://github.com/superset1/SQL/blob/master/MySQL_Create_db_hosts_for_iperf3.sql)
2. You need to change the values of the variables in /vars/main.yml file
3. Copy the /tests/test.yml file to the folder where you have a folder named "roles"
4. Write the following command on the command line: 
   ansible-playbook test.yml
5. Congratulations you did it!

NOTE:  You can rename test.yml file as you like 


Role Variables
--------------

See description for variables in /vars/main.yml file


Dependencies
------------

Don't need anything

Example Playbook
----------------

See the finished Playbook in folder tests

License
-------

MIT

Author Information
------------------

Hello, I'm Vitaly Kargin and I'm on my way to becoming a devops engineer!