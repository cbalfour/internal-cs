Automatic Marker
================

The automatic marker - aka automarker - is an extension to the UCT Vula
learning management system (LMS) to automatically mark programming
assignments. It usually appears as ``Automatic Marker`` in the left sidebar
of Vula course sites that use it. 

It is managed by the :ref:`scientific_officers` together with the
:ref:`sysadmins-label`.


.. warning:: The automatic marker is not currently zero-rated by South African mobile operators. To avoid data charges use Method 2 below.

Preparation
-----------

Before submitting you need to do the following:

#. Write and test your program on your workstation. 
   
   * If you are using the NetBeans IDE, be sure to remove the package name it adds from the top of the source file.

#. Put your uncompiled source files into a ``zip`` file.

   * The file name does not matter as long as it as a ``.zip`` extension.

   * The files must be in the root of the zip file, *not* in a folder unless a specific structure has been specified in the assignment question. 

Once you are ready to submit, select a method below.

Methods
-------

There are currently 2 methods for submitting your code to the automarker: ``Method 1`` and ``Method 2``. 

* ``Method 1`` is more interactive, but because it submits directly to the automarker (which is not currently zero-rated by mobile operators) will incur data charges.

* ``Method 2`` is less interactive as it uses a batch process, but because it submits to vula (which is zero-rated by most mobile operators) does not incure any data charges. 

**If the cost of data is an issue for you, please use Method 2.**


Method 1
########

This is the standard method for submitting to the automarker via its web interface. 

.. warning:: This method is not zero-rated by mobile operators.

#. Click on the ``Automatic Marker`` item on the left menu of the Vula site.

   * The assignment page - including the list of *Open Assignments* is displayed. Each open assignment should have a ``Browse`` and a ``Submit`` button.

#. Click on the ``Browse`` button of the assignment you want to submit and find and select the zip file you want to upload.

#. Click the ``Submit`` button to submit the assignment to the marker.

#. The automarker will mark the assignment providing feedback as it progresses. 

#. Examine the feedback, make the necessary changes to your program and follow this procedure again to submit an updated solution.

Method 2
########

.. note::Use this method to avoid data charges.


This is a 'batch' method to submit to the automatic marker. While 
it is less interactive, the same marking process is followed, 
and the results will be identical.

#. Click on ``Drop Box`` item on the left menu of the Vula site.

   * You should see an ``automark`` folder.

#. Open the ``automark`` folder.

   * You should see a folder for each assignment currently open e.g. ``Assignment 4: Control (if, for, while)``.

#. Open the folder for the assignment you wish to submit. 
   
   * The folder will usually be empty, unless there is a previous submission waiting to be processed. 
   * You can delete this file if you no longer want it to be processed, or keep it to be processed in addition to any new files you add.

#. Copy the zip file into the folder.

   .. note:: It can take **up to 30 minutes** for the file to be noticed and processed. Please be patient.
  
   * If there are other files in the folder that you still want processed, make sure you give the new file a different name.

#. When the automarker notices the zip file, it will process it in the same way it is processed in method 1.
    
#. Once processed, the zip file will be automatically removed and the feedback from automarker will be written to a ``.txt`` file e.g. ``05794891-399b-4c9d-8123-039d43bfc668.txt`` in the ``automark`` folder.


#. Examine the feedback file, make the necessary changes to your solution and follow this process again to submit a few solution.


Troubleshooting
---------------

* No ``Automatic Marker`` option on the Vula menu
  
  * This site / course does not use automatically marked assignments.

* No ``Drop box`` option on the Vula menu
  
  * This method has not yet been enabled. Contact the course convenor.

* No ``automark`` folder in your ``Drop box``
  
  * The Dropbox method is not fully active yet. Wait 30 minutes. If it 
    is still not active contact the course convenor.

* The folder for the assignment I want to submit does not yet exist in my ``Drop box`` ``automark`` folder
  
  * This could be because:

    * The assignment is not yet open: Check the open date and time in ``Assignments`` on the left Vula menu.
    * The assignment is closed: Check the close date and time in ``Assignments`` in the left Vula menu.
    * The automarker is still deploying the assignment to the Drop box: Wait 30 minutes.
