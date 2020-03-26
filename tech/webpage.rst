Personal Web Page
=================

How to build your personal web page.

Why do I need a Home Page?
--------------------------

Because it is your Internet contact card

How to setup my account to display my web page
----------------------------------------------

1) Log into the :ref:`shell` using your :ref:`cs_unix_credentials`.

2) Change directory to your ``public_html`` folder:

::

      [username@nightmare] ~$ cd public_html

3) Create the index.html file

    While you may create several Web pages, the index.html file will be your "landing page". This page will contain your primary information and links to other information that you may want to share.  
    
    Copy and save the following example html into your index.html file...

    .. code-block:: html

       <html>
               <head>
               <TITLE>Simple HTML Example</TITLE>
               </head>
               <body>
               <H1>HTML is Easy To Learn</H1>

               <P>The Internet contains a wealth of HTML learning resources.
               A simple search will yield the information you require.</P>
               </body>
       </html>

4) Making the index.html file to be readable

   Assuming that you are using the command line...

   View/List the content of the public_html directory::
   
   [username@nightmare] ~$ ls -lia

   Change the index.html file to be world readable::
  
   [username@nightmare] ~$ chmod 644 index.html

5) Viewing your website in the browser

    Browse to... http://www.cs.uct.ac.za/~<your_username>

Need help?
----------

Email the :ref:`sysadmins-label` as help@cs.uct.ac.za.


