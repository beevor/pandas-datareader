pandas-datareader
=================

Version 0.5.0 with daily.py modified to allow reading Google's financial data, although it seems to be hit and miss sometimes.
Currently using with zipline=1.1.1-np111py35_0, pandas=0.18.1/


Installation
------------


Install latest release version via pip
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. code-block:: shell

   $ pip install pandas-datareader

Install latest development version
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. code-block:: shell

    $ pip install git+https://github.com/pydata/pandas-datareader.git

or

.. code-block:: shell

    $ git clone https://github.com/pydata/pandas-datareader.git
    $ python setup.py install

Usage
-----

Starting in 0.19.0, pandas no longer supports ``pandas.io.data`` or ``pandas.io.wb``, so
you must replace your imports from ``pandas.io`` with those from ``pandas_datareader``:

.. code-block:: python

   from pandas.io import data, wb # becomes
   from pandas_datareader import data, wb

Many functions from the data module have been included in the top level API.

.. code-block:: python

   import pandas_datareader as pdr
   pdr.get_data_yahoo('AAPL')

See the `pandas-datareader documentation <https://pandas-datareader.readthedocs.io/>`_ for more details.
