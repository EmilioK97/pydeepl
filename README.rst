Note: The comercial `DeepL API <https://www.deepl.com/api.html>`_ has been released. You should use it instead subscribing to DeepL Pro.
========================================================================================================================================

pydeepl
=======
.. image:: https://api.travis-ci.org/EmilioK97/pydeepl.svg?branch=master


A Python API wrapper for the `DeepL <https://www.deepl.com/>`_ translation service.

Installation
------------

.. code:: python

    pip install pydeepl

Getting Started
---------------

Python Version
~~~~~~~~~~~~~~

Pydeepl was written for both Python 2 and Python 3.

Add pydeepl to your application
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. code:: python

    import pydeepl

    sentence = 'I like turtles.'
    from_language = 'EN'
    to_language = 'ES'

    translation = pydeepl.translate(sentence, to_language, from_lang=from_language)
    print(translation)

    # Using auto-detection
    translation = pydeepl.translate(sentence, to_language)
    print(translation)

Supported Languages
-------------------

Pydeepl supports these languages:

+--------+-----------------+
| Code   | Language        |
+========+=================+
| auto   | *Auto detect*   |
+--------+-----------------+
| DE     | German          |
+--------+-----------------+
| EN     | English         |
+--------+-----------------+
| FR     | French          |
+--------+-----------------+
| ES     | Spanish         |
+--------+-----------------+
| IT     | Italian         |
+--------+-----------------+
| NL     | Dutch           |
+--------+-----------------+
| PL     | Polish          |
+--------+-----------------+
| PT     | Portuguese      |
+--------+-----------------+
| RU     | Russian         |
+--------+-----------------+

    Note that auto detection is only possible for the source language.

Disclaimer
----------

DeepL is a product from DeepL GmbH. More info:
`deepl.com/publisher.html <https://www.deepl.com/publisher.html>`__

This package has been heavily inspired by
`node-deepls <https://github.com/pbrln/node-deepl>`__ and
`DeepLy <https://github.com/chriskonnertz/DeepLy>`__.

License
-------

This project is licensed under the MIT License - see the
`LICENSE <LICENSE>`__ file for details
