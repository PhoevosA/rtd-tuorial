Configure workspace
===================

.. _setupGuide:

SPLICE Project Setup Guide
--------------------------

.. _prerequisites:

Prerequisites
-------------

   * Python 3.8 or higher
   * ``uv`` package manager

.. code-block:: console

   curl -LsSf https://astral.sh/uv/install.sh | sh

Project Structure
-----------------


The project consists of four main components:

   * \ ``splice-api``\: FastAPI-based REST API service
   * ``splice-cli``: Command-line interface tool
   * ``splice-lib``: Core library package
   * ``splice-pipeline``: Analytics pipeline application

Project Components
------------------

1. API Service
^^^^^^^^^^^^^^

To run the FAstAPI development server:

.. code-block:: console

  cd splice-api
  uv run fastapi dev

2. Command Line Interface (CLI)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Installation

.. code-block:: console

  cd splice-cli
  uv pip install -e . 

Usage

.. code-block:: console

  uv run splice-lib

Managing Dependencies
---------------------

Adding Dependencies to Sub-Projects
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

To add dependencies to individual sub-projects (api, cli or lib):

1. Navigate to the sub-project directory:

.. code-block:: console

  cd splice-cli # Example for CLI component

2. Add the desired package:

.. code-block:: console

  uv add <package-name> # Example: uv add typer

The package will be automatically added to the sub-project's ``pyproject.toml`` file.

Adding Dependencies to Parent Project
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

To add dependencies that should be available to cross all sub-projects:

1. From the root ``splice`` directory:

.. code-block:: console

  uv add <package-name> # Example: uv add pytest

This will add the package to the parent project's ``pyproject.toml`` file.
