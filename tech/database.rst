.. _database-label:
.. _database:

Database
============

A MySQL database service is available on the :ref:`shell`

For other database requirements, please contact the :ref:`sysadmins`

MySQL (on nightmare)
--------------------

This section describes how to setup your MySQL database on the shell server.

#. SSH into the :ref:`shell`

#. Create your mysql database, username and password by running the following command::

    mysqluser

This should output something similar to the following which includes 
your database name, username and password:

.. code-block:: sh

    MySQL:
    hostname: nightmare.cs.uct.ac.za
    database: smtdoe004
    username: smtdoe004
    password: wohgefee
    You can set your new password with:

    mysql --user=smtdoe004 --password=wohgefee smtdoe004
    mysql> set password=password('your new pass');
    mysql> quit

.. note:: Take note of hostname, database, username and password for all future use. 

.. note:: If you forget the password, just re-run mysqluser and it will give you a new random password without deleting your existing database.

