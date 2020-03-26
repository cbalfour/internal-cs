.. _email:

Email
=====

.. toctree::
   :maxdepth: 2
   :caption: Contents:

   out-of-office 


The Department of Computer Science operates its own email service, separate and in addition to the email service provided centrally by the University of Cape Town. This service is available to all Computer Science staff, graduate students and undergraduate students from their second year of study.

This email service consists of the following:

*    A cs.uct.ac.za domain email address;
*    A mailbox accessible via an email client using the IMAPs or POP3s protocols, or via the Department's web interface;
*    A web mail interface;
*    A mailing list server;
*    A SMTP server for sending email from on and off-campus.

Policies
++++++++

This service is subject to the following policies:

*    Relevant University of Cape Town's `policies`_.
*    A disk-space usage quota.

Accessing Email
+++++++++++++++

There are three methods for accessing your email:

*    Webmail interface, recommended primarily for off-campus access e.g. when travelling overseas, or using public computing facilities such as internet cafes.
*    Email client, recommend for on-campus use.
*    Direct mailbox access using a text-based email client on the unix shell server. This is an advanced option only recommended for unix users familiar with the unix command-line interface.

Webmail Interface
-----------------

A webmail interface is available at `webmail.cs.uct.ac.za`_.

This interface can be used to access your email from any computer with internet access and a web browser. No other software or configuration is required.

The web interface is recommended for use from off-campus and when using insecure shared facilities such as internet cafes.

The web interface is not recommended for use from department facilities. Within the Department, we recommend that you use an email client.
 
Email Client
------------

An email client is the recommended method for accessing your email from Departmental facilities.

While any email client that supports SMTP and IMAPs can be used, we recommend that you use one of the following supported email clients:

*    Mozilla Thunderbird
*    Microsoft Outlook
*    mutt

To access email in your mailbox using IMAPs configure your email client with the following settings:

    Server: ``imap.cs.uct.ac.za``
    Require secure connection using either SSL or TLS. This setting is usually hidden away under Advanced configuration.
    Authentication using your :ref:`cs_unix_credentials`.

To send email from on-campus you should configure your email client to use the following outgoing SMTP settings. From home you can either use these settings or your internet service providers (ISP) SMTP settings:

    Server: ``smtp.cs.uct.ac.za``
    Require secure connection using either SSL or TLS. This setting is usually hidden away under Advanced configuration
    Require authentication
    Authenticate using your :ref:`cs_unix_credentials`.

Unix Shell
----------

It is also currently possible to access your mailbox as a local Maildir folder from the Departmental :ref:`shell` using the following available text-based email clients:

*    alpine (similar to the deprecated Pine email client)
*    mutt

These clients can also be configured to access your mailbox via IMAPs using the settings described in the email client section.

This method should only be used by people familiar with the unix command-line interface and text-based email clients.

Other Features
--------------

    You can automatically forward your email to another email address by creating a ``.forward`` file.

    Out-of-the-office reply. You can set an `out-of-the-office reply`_ - also known as a  vacation message - to notify people when you are away from from the office.

About
+++++

Our mail service is built using standard protocols and the following open-source software:

*    Linux operating system
*    Exim mail transport agent
*    Courier IMAP server
*    Mailman mailing list manager
*    Squirrelmail and Roundcube webmail interfaces 

.. _policies: http://www.uct.ac.za/main/about/policies
.. _`webmail.cs.uct.ac.za`: https://webmail.cs.uct.ac.za/
.. _`out-of-the-office reply`: out-of-office
