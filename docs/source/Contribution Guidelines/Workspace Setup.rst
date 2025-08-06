SPLICE workspace setup guide
============================

This document gives a step-by-step guide on how to set up your workspace for contributing to the SPLICE project. It covers the necessary tools, configurations, and best practices.

Pre-Requisites
--------------
Before you begin, ensure you have the following installed on your machine:

* Git: Version control system to manage your code.
* Python: Programming language used in the SPLICE project.
* IDE: An Integrated Development Environment (IDE) like VSCode or Jupyter Notebook for writing and testing code.

Set Up SPLICE Workspace
-----------------------

Clone the SPLICE Repository
^^^^^^^^^^^^^^^^^^^^^^^^^^^

1. Open your terminal or command prompt.

2. Navigate to the directory where you want to clone the SPLICE repository

3. Run the following command to clone the repository:

.. code-block:: console

  git clone https://github.com/Beatson-CompBio/SPLICE.git

4. Change into the cloned directory:

.. code-block:: console

  cd SPLICE

Create a new branch
^^^^^^^^^^^^^^^^^^^

1. *Recommended*: To work on a new feature or fix a bug, create a new branch from the ``feature/*``, ``bugfix/*``, or ``hotfix/*`` remote branches. Use the following command to create and switch to a new branch:

.. code-block:: console

  git checkout -b local-branch-name remotes/origin/remote-branch-name

2. In case branches with names like ``feature/*`` or ``bugfix/*`` does not exist, we recommend having a discussion with our team before creating a new feature branch. Once that is done, you can create a new branch with the following command:

.. code-block:: console 

  git checkout -b my-feature-branch

3. When you raise a pull request, your code will be merged into the codebase based on the branching convention and rule sets. Find out more details on our branching convention and rule set :doc:`here <Branching Convention>`.

Configure your workspace
^^^^^^^^^^^^^^^^^^^^^^^^

1. Detailed steps for configuring SPLICE workspace can be found in the :ref:`link <configureWorkspace>`.

Add you code and commit changes
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

1. After makign changes to the code, add the files you want to commit individually t oavoid losing changes in future, in case of rollback. Use the following command:

.. code-block:: console

  git add path/to/your/file

2. Commit your changes with a descriptive message:

.. code-block:: console

  git commit -m "Your descriptive commit message"

3. Push your changes to the remote repository:

..  code-block:: console

  git push # in case of existing remoe branch 

OR

.. code-block:: console

  got push origin my-feature-branch # in case of new branch

Create a pull request 
^^^^^^^^^^^^^^^^^^^^^

1. Go to the GitHub repository page for SPLICE.
2. Click on the "Pull requests" tab.
3. Click on the "New pull request" button.
4. Select your branch from the dropdown menu.
5. Review the changes and add a descriptive title and comment for your pull request.
6. Click on the "Create pull request" button to submit your changes for review.

You can find more details on our PR guidelines :doc:`here <Pull Request (PR) Guidelines>`.
