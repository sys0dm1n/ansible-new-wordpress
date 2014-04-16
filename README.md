Role Name
========

Download wordpress 3.8.3 to the documentroot, creates MySQL database and create the Virtualhost for Apache.
All you still need to do is enabling the virtualhost like follow:
 sudo a2ensite {{virtualhost_file_name}}
 sudo service apache2 reload

Requirements
------------

You should have Apache2, mysql-server and php5 pre installed

Role Variables
--------------
* RootFolder: The folder name where the wordpress code will be stored
* wp_db_name: The Wordpress database name
* wp_db_user: The Wordpress database username
* wp_db_password: The Wordpress database password
* mysql_user: Root username
* mysql_password: Root password
* wp_version: Wordpress version
* wp_sha256sum: The Wordpress sha 256 checksum
#### Apache Virtualhost variables:
* server_hostname: Website's domain name
* server_alias: Website's domain alias

Example Playbook
-------------------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      sudo: yes
      roles:
         - new-wordpress

License
-------

BSD

Author Information
------------------

sys0dm1n
http://terraltech.com/
