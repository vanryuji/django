# Overview
Persistent connections avoid the overhead of re-establishing a connection to the database in each request. They’re controlled by the CONN_MAX_AGE parameter which defines the maximum lifetime of a connection. It can be set independently for each database.

The default value is 0, preserving the historical behavior of closing the database connection at the end of each request. To enable persistent connections, set CONN_MAX_AGE to a positive number of seconds. For unlimited persistent connections, set it to None.


# Environments
* Django 2.0


# Reference
* https://docs.djangoproject.com/en/2.0/ref/databases/
