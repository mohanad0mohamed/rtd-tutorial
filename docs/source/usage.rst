Usage
=====

.. _installation:

Installation
------------

To use Mohanad, first install it using pip:

.. code-block:: console

   (.venv) $ pip install mohanad

Creating recipes
----------------

To retrieve a list of random ingredients,
you can use the ``mohanad.get_random_ingredients()`` function:

.. autofunction:: mohanad.get_random_ingredients

The ``kind`` parameter should be either ``"script"``, ``"vcs"``,
or ``"doc"``. Otherwise, :py:func:`mohanad.get_random_ingredients`
will raise an exception.

.. autoexception:: lumache.InvalidKindError

For example:

>>> import mohanad
>>> mohanad.get_random_ingredients()
['python', 'git', 'markdown']

