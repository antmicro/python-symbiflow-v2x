Full Adder Example
++++++++++++++++++

An example of the classical combinational `"full adder" <https://en.wikipedia.org/wiki/Adder_(electronics)#Full_adder>`_ circuit shown in |fig60|_ of the `"Combinational block" <https://docs.verilogtorouting.org/en/latest/tutorials/arch/timing_modeling/#combinational-block>`_ section in the Primitive Block Timing Modeling Tutorial of the Verilog to Routing documentation and reproduced below.

.. |fig60| replace:: ``Figure 60 - Full Adder``
.. _fig60: https://docs.verilogtorouting.org/en/latest/tutorials/arch/timing_modeling/#combinational-block

.. image:: full-adder.svg
   :alt: Figure 59 from Verilog to Routing Documentation

*Fig. 59 - Full Adder*

|

.. symbolator:: adder.sim.v

.. verilog-diagram:: adder.sim.v
   :type: netlistsvg
   :module: ADDER

|

.. no-license::  adder.sim.v
   :language: verilog
   :caption: adder.sim.v

.. no-license:: adder.model.xml
   :language: xml
   :caption: adder.model.xml

.. no-license:: adder.pb_type.xml
   :language: xml
   :caption: adder.pb_type.xml


Detection of combinational connections
**************************************

* Output has combinational connection with input

Blackbox detection
******************

* Model of the leaf ``pb_type`` is generated
* Leaf ``pb_type`` XML is generated

Timings
*******

* All the timings defined for wires with attributes should be included in ``pb_type`` XML
