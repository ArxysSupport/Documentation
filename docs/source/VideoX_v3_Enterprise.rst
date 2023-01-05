Arxys Video X v3 Enterprise
=====

.. _installation:

Quick Installation Guide
------------


#. Unpack the components
	* Carefully remove the VideoX v3 Enterprise Appliance from its shipping box. The VideoX v3 Enterprise Appliance is shipped without its hard drives installed. Operating system SSDs or database SSDs are shipped installed. 

#. Install the Rackmount Kit on the Chassis
	* A rackmount rail kit is included with VideoX v3 Enterprise Appliance. Refer to the documentation shipped inside the rackmount rail kit box.

#. Cabling VideoX v3 Enterprise 
	* The VideoX v3 Enterprise Appliance requires two AC power sources. Connect both power cords. Only connect a display to the VGA port. Connect a keyboard and mouse to any available USB port. Network connectivity is required during the operation of the VideoX V3 Enterprise. Plug in at least one Ethernet cable into an Ethernet port of the VideoX V3 Enterprise. A network cable should also be connected to the management port for later usage.

.. code-block:: console

   (.venv) $ pip install lumache

Creating recipes
----------------

To retrieve a list of random ingredients,
you can use the ``lumache.get_random_ingredients()`` function:

.. autofunction:: lumache.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`lumache.get_random_ingredients`
will raise an exception.

.. autoexception:: lumache.InvalidKindError

For example:

>>> import lumache
>>> lumache.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']
