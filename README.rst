======================
 oberon00 user manual
======================

+-------------------+----------------------------------------------------------+
| **Title**         | oberon00 (Oberon-0 subset for use as a hardware-software |
|                   | description language)                                    |
+-------------------+----------------------------------------------------------+
| **Author**        | Nikolaos Kavvadias (C) 2004, 2005, 2006, 2007, 2008,     |
|                   | 2009, 2010, 2011, 2012, 2013, 2014                       |
+-------------------+----------------------------------------------------------+
| **Contact**       | nikos@nkavvadias.com                                     |
+-------------------+----------------------------------------------------------+
| **Website**       | http://www.nkavvadias.com                                |
+-------------------+----------------------------------------------------------+
| **Release Date**  | 20 September 2014                                        |
+-------------------+----------------------------------------------------------+
| **Version**       | 0.2.0                                                    |
+-------------------+----------------------------------------------------------+
| **Rev. history**  |                                                          |
+-------------------+----------------------------------------------------------+
|        **v0.2.0** | 2014-09-20                                               |
|                   |                                                          |
|                   | Updated for github. Added AUTHORS, LICENSE, README,      |
|                   | VERSION. The compiled tables file (oberon00.cgt) has     |
|                   | been removed from the distribution.                      |
+-------------------+----------------------------------------------------------+
|        **v0.1.0** | 2004-10-31                                               |
|                   |                                                          |
|                   | Initial version as submitted to GOLD Parsing System's    |
|                   | developer, Devin Cook (Devin@GOLDparser.org). Translated |
|                   | the Oberon-00 EBNF to a regular BNF in the GOLD parser   |
|                   | style.                                                   |
+-------------------+----------------------------------------------------------+


1. Introduction
===============

Oberon-00 is a simple programming language proposed in [Wirth98]_ as a 
simple example of a common language that can be used for hardware and
software compilation. Such language has been used for experimentation and 
research (establishing a proof-of-concept) purposes in the field of high-level 
synthesis (HLS) and as a testbed for hardware-software codesign. Oberon-00 is 
derived as a hardware-friendly subset of Oberon.

Oberon-00 has been used as a source language for describing simple programs that 
are mapped by a hardware compiler (namely ``hwcomp``) to Xilinx XNF netlist 
format. ``hwcomp`` is an implementation of a hardware compiler inspired Wirth's 
hardware compilation article. The compiler was reportedly written in August 
1998. The program is similar to the one described in the article by Niklaus 
Wirth. It takes a Pascal-esque/Oberon program as input and produces an XNF 
netlist as an output. The compiler has logic to generate all common operations: 
``*, /, -, +, >=, <=, <, >, =``.

The original source of the ``hwcomp`` project as well as the link to the source 
code download are now dead:

- http://www.valavan.net/hwcomp.html (DEAD LINK)
- http://www.valavan.net/hwcomp.zip (DEAD LINK)

However, an archived link to the main webpage for this project has been made 
accessible:

- https://web.archive.org/web/20080130031832/http://valavan.net/hwcomp.html

This package contains both a regular BNF grammar derived from the Oberon-00 
EBNF, which can be used within the GOLD parser environment and the original 
EBNF. It does not contain the ``hwcomp`` source code itself.

A former version of this file collection can also be downloaded from the GOLD 
Parsing System's website: http://goldparser.org


2. File listing
===============

The ``oberon00`` file collection includes the following files: 

+-----------------------+------------------------------------------------------+
| /oberon00             | Top-level directory                                  |
+-----------------------+------------------------------------------------------+
| AUTHORS               | List of authors.                                     |
+-----------------------+------------------------------------------------------+
| LICENSE               | License argeement (Modified BSD license).            |
+-----------------------+------------------------------------------------------+
| README.rst            | This file.                                           |
+-----------------------+------------------------------------------------------+
| README.html           | HTML version of README.                              |
+-----------------------+------------------------------------------------------+
| README.pdf            | PDF version of README.                               |
+-----------------------+------------------------------------------------------+
| VERSION               | Current version.                                     |
+-----------------------+------------------------------------------------------+
| first.obr             | Example program 1.                                   |
+-----------------------+------------------------------------------------------+
| log.obr               | Example program 2.                                   |
+-----------------------+------------------------------------------------------+
| minmax.obr            | Example program 3.                                   |
+-----------------------+------------------------------------------------------+
| multiply.obr          | Example program 4.                                   |
+-----------------------+------------------------------------------------------+
| oberon00.grm          | The GOLD parser grammar for Oberon-00 [GPS]_.        |
+-----------------------+------------------------------------------------------+
| oberon00.ebnf         | An EBNF for Oberon-00.                               |
+-----------------------+------------------------------------------------------+
| second.obr            | Example program 5.                                   |
+-----------------------+------------------------------------------------------+

3. Usage
========

Detailed usage details in context of the GOLD Parsing System (previously known 
as the GOLD Parser Builder) have been left as a TODO. 


4. References
=============

.. [Wirth98] Niklaus Wirth, "Hardware Compilation: Translating Programs into 
   Circuits," IEEE Computer, Vol. 31, No. 6, pp. 25--31, June 1998.

.. [GPS] Devin Cool, The GOLD Parsing System/Parser Builder,
   http://www.goldparser.org
