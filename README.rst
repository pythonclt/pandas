Pandas Vincent Vega D3 and Me and You and Your Cousin Too
=========================================================

.. image:: http://i.imgur.com/1NTMQko.png

Generating data visualizations programmatically is fun heya!

- It's a process:

  * Acquire - Parse - Filter - Mine - Represent - Refine - Interact
  * Ben Fry in *Visualizing Data* (O'Reilly)

- What can be done with some of these tools?
- Simple examples of Vega usage

----------

Pandas
------

Open source library with data structures and data analysis tools for Python.

- DataFrame object for data manipulation
- Time series data functionality

DataFrame
~~~~~~~~~

A 2D labeled data structure with columns of potentially different types.

- Like a spreadsheet or SQL table, or a dict of Series objects
- Can pass in index and columns args (row and column labels)

Series
~~~~~~

A one-dimensional labeled array capable of holding any data type.

- The axis labels together are called the index
- Will automatically missing data (NaN)


Vincent
-------

.. image:: http://cl.ly/TUDZ

Helps ease building of visualizations on top of D3 with Vega.

- Python data power, JavaScript visualization power
- Understands Pandas DataFrames and Series

Vega
----

A visualization grammar for creating and saving visualization designs.

- Declarative format
- Describe data visualizations in JSON
- Generate interactive views using HTML5 Canvas or SVG

Vega Runtime
~~~~~~~~~~~~

Parses Vega specifications to produce interactive visualizations.

- With node.js can be run server-side to render specs to PNG or SVG
- Can also use the CLI tools `vg2png` and `vg2svg`
- Parser turns the JSON spec into a constructor for `View` objects (JS)
- Actual visualizations are instances of the `vg.View` class (JS)

Vega Specification
~~~~~~~~~~~~~~~~~~

A Vega spec is simply JSON that describes the design of a **Visualization**

  * The data sets used
  * Scale transforms
  * Encoding algorithms
  * Axes
  * Visual marks (e.g. lines, shapes)

- The specs are read and interpreted by the runtime to dynamically create viz
  (and more)

Vega Visualization
~~~~~~~~~~~~~~~~~~

The top-level object in Vega - the container for all visual elements.

- Consists of:

  * A rectangular canvas, where the visual elements live
  * A viewport, a window to that canvas

- Basic properties, such as the view's width and height
- Definitions for:

  * The **Data** to visualize
  * **Scales** that map data values to visual values
  * **Axes** that visualize the scales (as ticks, labels)
  * Graphical **Marks** (shapes, arcs, etc) that visualize the data

.. image:: http://cl.ly/TUPx

D3
--

JavaScript library that provides visualization components and a data-driven
approach for manipulating the DOM.

- Based on web standards (CSS3, HTML5, SVG)
- Focuses on the efficient manipulation of documents based on data
- Allows styles, attributes etc to be specified as *functions* of data
- Provides graphical primitives for charts (area, line, pie)
- Essentially a low-level library that can be used to build upon

Tools
-----

Many good tools / libs / environments available.

- IPython: interactive shells; browser-based notebook
- NumPy: scientific computing with Python
- Anaconda: cross-platform distribution for data analysis etc
- Enthought: another cross-platform distribution; Canopy, EPD products


.. _ipython_url: http://continuum.io/downloads

.. _ipython_notebook_gallery: http://git.io/E3zt3w

.. _numpy_url: http://www.numpy.org/

.. _pandas_url: http://pandas.pydata.org/

.. _vincent_url: https://github.com/wrobstory/vincent

.. _vega_url: https://github.com/trifacta/vega

.. _d3_url: http://d3js.org/

.. _anaconda_url: https://store.continuum.io/cshop/anaconda/

.. _enthought_canopy_url: https://www.enthought.com/products/canopy/

.. _enthought_epd_url: https://www.enthought.com/products/epd/
