SPLICE Documentation
====================

**SPLICE** (Scientific Platform for Life sciences data Integration, Collaboration and Exploration) is a data platform which supports the collection, storage, organisation, processing, analysis and visualisation of experimental data across research areas in life sciences. SPLICE is aimed at enhancing collaboration between researchers enabling easy alignment to FAIR data principles.

Contents
--------
  * :ref:`Why use SPLICE <YSPLICE>`
  * :ref:`Design Aims <dAims>`
  * :ref:`Installation <installation>`
  * :ref:`Usage <usage>`



.. _YSPLICE:

Why use SPLICE
--------------
...

.. _dAims:

Design Aims
-----------
**High-data volume and throughput**: Can store and organise 100’s – 1000s TB of research data in a multitude of formats in a structured and open DB which can be queried. Upload, analysis and display needs to achieve a ‘useable’ latency.

**Consistent metadata formatting and vocabulary**: Enables and enforces (via QA checks) that data and metadata are created, stored and presented consistently ideally with established data models (OMOP).

**Enables end-user creation, read, update of data/metadata**: Authorised end-users can upload data from their own labs, they can share and read all data, update their own data or remove it from the service.

**Follow Infrastructure as code (IaC) principles**: We want to build a system that we can easily deploy internally during testing but also on commercial and national scale academic infrastructure easily.

**Transparent design choices and up-to-date documentation**: Design choices are documented early in the project in a way that can be shared with the wider stakeholders. Documentation is kept up to date. We communicate early what we are planning to avoid surprises and set expectations.

**Automated analysis pipelines**: Makes use of established libraries for analysis and automated workflows (nextflow) at ingestion and on demand(?).

**CI/CD**: Testing and validation is a primary concern from the start. Testing is automated and fixes are automatically deployed.

**ML/AI Ready**: Platform design anticipates and enables future application of ML model by providing curated training data on demand.

.. _installation:

Installation
------------

...

.. _usage:

Usage
-----
...

.. note::

   This project is under active development.

.. toctree::
 :maxdepth: 1 
 :hidden:
 :glob:

 Wiki
 SPLICE workspace setup guide <Contribution Guidelines/Workspace Setup>
 Contribution Guidelines/*
 Installation/*
 Naming Standards/*
 System Infrastructure/*
 Testing Guides/*
 extra/*
