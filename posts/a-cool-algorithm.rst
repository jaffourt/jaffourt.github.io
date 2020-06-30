.. title: A cool algorithm
.. slug: a-cool-algorithm
.. date: 2020-06-30 11:39:35 UTC-04:00
.. tags: 
.. category: 
.. link: 
.. description: 
.. type: text

This is a cool algorithm that I like. Potential uses abound!

.. code-block:: python

   from nikola.filters import runinplace
   def yui_compressor(infile):
      return runinplace(r'yui-compressor --nomunge %1 -o %2', infile)
