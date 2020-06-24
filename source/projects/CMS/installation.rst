Installation
============

The portal is primarily a django based application, and to set it up we
require to have python environment with django and other project
dependencies installed. Though one can work with the project without an
virtual environment, it is recommended to use one so as to avoid
conflicts with other projects.

1. Make sure that you have ``Python 3``, ``python-3-devel``, ``gcc``,
   ``virtualenv``, and ``pip`` installed.
2. Clone the repository

.. code:: bash

   $ git clone https://github.com/amfoss/cms.git
   $ cd cms

3. Create a python 3 virtualenv, and activate the environment.

.. code:: bash

   $ virtualenv -p python3 .
   $ source bin/activate

4. Install the project dependencies from ``requirements.txt``

.. code:: bash

   $ pip install -r requirements.txt

After Setting up
----------------

From now when you start your work, run ``source bin/activate`` inside
the project repository and you can work with the django application as
usual - - ``python manage.py migrate`` - set up database -
``python manage.py createsuperuser`` - create admin user -
``python manage.py runserver`` - run the project locally

*Make sure you pull new changes from remote regularly.*