Role Name
=========

Installs Jekyll https://jekyllrb.com/

Transform your plain text into static websites and blogs.

Requirements
------------

Install Jekyll role
````
sudo ansible-galaxy install -r requirements.yml -f
````

Vagrant
-------
Spin up Environment under Vagrant to test.
````
vagrant up
````

Docker
------
Spin up Docker container for testing (With NGINX)
````
docker run -d -p 80:80 -p 4000:4000 mrlesmithjr/jekyll
````

Role Variables
--------------

None

Dependencies
------------

ansible-nginx (Installed as part of requirements.yml)

Example Playbook
----------------

###### Galaxy
    - hosts: servers
      roles:
         - role: mrlesmithjr.jekyll

###### GitHub
    - hosts: servers
      roles:
        - role: ansible-jekyll

License
-------

BSD

Author Information
------------------

Larry Smith Jr.
- @mrlesmithjr
- http://everythingshouldbevirtual.com
- mrlesmithjr [at] gmail.com
