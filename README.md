osTicket-Addons
===============

Info
====
Round robin user asignation: this addon is used to automatically assign new tickets to a group of users.

Requirements
============
-	Working osTicket versions:
  - v1.9.2
  - v1.9.3
- You need to create a database table called "okm_assigner" with this definition
````sql
CREATE TABLE okm_assigner (
  id tinyint(4),
  tickets int(11),
  mail varchar(50),
  active tinyint(1) COLLATE utf8_bin DEFAULT NULL
);
````
