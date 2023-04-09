Context
=========

I wanted to learn how to use Ansible and took this [lesson](https://openclassrooms.com/fr/courses/2035796-utilisez-ansible-pour-automatiser-vos-taches-de-configuration).
<br/>Deploying a Wiki on your servers is now an easy and quick task thanks to Ansible. You can easily personalize the scripts of this one to serve your own purpose.

Roles
-----

<p>5 Roles have been created (2 roles of installation and 3 roles of configuration)</p>
apache : to install apache packages
<br>mariadb: to install mariadb packages
<br/>Mediawiki: Configuration of our Wiki
<ul>
<li>commun: all common variables used in configuration roles</li>
<li>confapache: Apache configuration</li>
<li>confmariadb: MariaDB configuration</li>
</ul>

Dependencies
------------

An inventory file containing all your nodes. I organized my nodes by groups in case I add other servers.

Playbooks
---------

3 Playbooks have been made to install the different components: Apache, MariaDB, MediaWiki