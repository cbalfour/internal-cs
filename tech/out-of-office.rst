Out-of-Office Message
=====================

You can setup an out-of-the-office reply - also known as a vacation message - to notify people who send you email that you are away from the office.

To setup your out-of-office reply do the following:

1. Log into the :ref:`shell-label` using ssh.

2. Create a file called ``.vacation.msg`` to contain the email you want to have automatically emailed. The contents of the file should look similar to the following:

::

   Subject: Out of the office
   
   I will be away from the office from 1 January 2020 to 31 December 2020.
   I am unlikely to read email during this time. 
   
   I will attend to all email on my return.
   
Note the blank line between Subject and I will attend...

3. Create a ``.forward`` file similar to the following::

    \username, "|/usr/bin/vacation username"


In step 3 above, replace username with your username.

The ``\username`` option tells the mail server to keep a copy of the email in your local mailbox. If you would like to forward your email to another email address while you are way, replace ``\username`` with an email address.


