5minbootstrap
=============

This is a fork from https://github.com/phred/5minbootstrap I use to secure my Ubuntu EC2 instances. 

Steps to reuse:

* edit `hosts.ini` and set your ec2 instance name
* edit `config/postfix_selections` to set domains for email 
* set Amazon AWS keys to your ssh repository:

    ssh-agent
    
    ssh-add ~/path/to/foo.pem

* Run the ansible steps:

    ansible-playbook -i hosts.ini bootstrap.yml -u ubuntu --sudo


Sources
=========

The original source:

https://github.com/phred/5minbootstrap


This excellent post:

http://plusbryan.com/my-first-5-minutes-on-a-server-or-essential-security-for-linux-servers


A blog post that the original author wrote to go along with this.  Check it out!

http://practicalops.com/my-first-5-minutes-on-a-server.html



