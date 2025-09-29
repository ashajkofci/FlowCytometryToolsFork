.. _install:

How to install?
----------------

FlowCytometryTools targets `Python 3.9+ <https://www.python.org/getit/>`__ and depends on
the scientific Python stack. The minimum tested versions for Python 3.12 are:
`numpy (>=1.26) <https://numpy.org/>`__,
`pandas (>=2.1) <https://github.com/pandas-dev/pandas>`__,
`scipy (>=1.12) <https://www.scipy.org/>`__,
`matplotlib (>=3.8) <https://matplotlib.org/>`__ and
`fcsparser (FlowCytometryTools fork) <https://github.com/ashajkofci/fcsparser>`__.

#. Creating an isolated environment such as `conda <https://www.anaconda.com/download/>`_
    or `venv <https://docs.python.org/3/library/venv.html>`_ is recommended before
    installing the dependencies.

#. Optional: if you intend to use the FlowCytometryTools GUI for drawing gates you'll also need to install `wx-python <https://wiki.wxpython.org/How%20to%20install%20wxPython>`_.

#. Go to your command terminal and enter the following:

   .. code-block:: bash

    pip install flowcytometrytools

    The project provides a ``pyproject.toml`` build definition, so editable installs for
    development are also supported:

    .. code-block:: bash

        pip install -e .

    When installing from source, pip will automatically fetch the ``ashajkofci/fcsparser``
    fork to ensure compatibility with NumPy 2.x. If you maintain your own environment,
    make sure no older ``fcsparser`` release that depends on ``numpy<2`` is pinned.

(Note: Please do not use ``sudo`` when installing with pip. Instead figure out
how to use virtual environments or conda.)

That's it!
