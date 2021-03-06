.. processRuns documentation master file, created by
   sphinx-quickstart on Fri Jan 22 14:38:46 2016.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to OVERWATCH documentation!
=======================================

ALICE **OVERWATCH**: Online Visualization of Emerging tRends and Web Accessible deTector Conditions using the HLT.

Welcome to OVERWATCH, an online monitoring framework utilizing detector histograms provided by the HLT. The OVERWATCH framework processes these histograms and displays them minute-by-minute on this website; this allows for real-time monitoring of detector performance, effortlessly available to any ALICE member at any location. For example, a collaborator in the US can monitor the EMCal trigger patch ADC spectrum for noisy TRUs in the comfort of daylight hours, while the CERN-based detector expert sleeps.

The framework also features the ability to automate QA functions to identify detector performance problems, as well as the ability to examine detector behavior during user-specified time ranges within a run. Moreover, the framework provides long-term trending info, i.e. the ability to plot detector quantities as a function of run number. OVERWATCH complements the DQM framework, allowing remote monitoring and easily implementable user customization. We provide extensive documentation for any detector system to be easily added to OVERWATCH, and encourage more subsystems to take advantage of the framework. For more information, see `detector modules`_.

Please see the README_ for information about the project, and how to use it. The code is available at `raymondEhlers/OVERWATCH`_.

.. _README: README.html
.. _raymondEhlers/OVERWATCH: https://github.com/raymondEhlers/OVERWATCH

.. include:: linksBackToApp.rst

Process Runs
============

The main processing function: takes ROOT files from the HLT viewer and organizes them into a run
directory and subsystem structure, then writes out histograms to the webpage.  

.. toctree::
   :maxdepth: 2

   processRuns

Modules
-------

These powerful modules provide much of the processing functionality for Process Runs. They also
provide a number of helper functions for detector-specific processing.

.. toctree::
   :maxdepth: 2

   processRunsModules

Detector Modules
----------------

These modules provide detector-specific functionality, allowing organization of histograms, as
well as functions to check QA, among many other possible features.

.. toctree::
   :maxdepth: 2

   processRunsModules.detectors

Web App
=======

The web app provides interactive access to the processing capabilities and output from Process Runs.
It can work both through WSGI, as well as a standalone server.

.. toctree::
   :maxdepth: 2

   webApp

Modules
-------

These modules provide support functions for the Web App, including authentication and validation
of inputs for safe operation.

.. toctree::
   :maxdepth: 2

   webAppModules

Configuration
=============

Provides convenient configuration for both Process Runs and the Web App.

.. toctree::
   :maxdepth: 2

   config

Back to the Web App
===================

.. include:: linksBackToApp.rst

---------------------

Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`

