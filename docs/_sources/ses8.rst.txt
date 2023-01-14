Session 8 - Encapsulation
=========================

In Python, it is generally considered best practice to make all attributes public unless there is a specific need to make them private. This is in contrast to languages like Java, where private attributes and accompanying getters and setters are the norm.

When we need to encapsulate data (e.i if we need to validate the data) we can use different methods. We will look at one approaches: propertie.

A property is a build in decorator function and is using the syntax :code:`@property`. Just like you learned in the session about decorator functions. Descriptor classes is a class with the :code:`__get__(), __set__() and __deleter__()` methods implemened.

This approach is considered best practice or 'Pythonic' and this is what we will look at in todays session.

.. quote::
   A property, in some object-oriented programming languages, is a special sort of class member, intermediate in functionality between a field (or data member) and a method. The syntax for reading and writing of properties is like for fields, but property reads and writes are (usually) translated to 'getter' and 'setter' method calls. The field-like syntax is easier to read and write than many method calls[citation needed], yet the interposition of method calls "under the hood" allows for data validation, active updating (e.g., of GUI elements), or implementation of what may be called "read-only fields".

.. The pythonic approach starts out with the quite bold statement that all attributes are public, and unless specificly needed there are not any reason to make them anything else but public. If you think on back on your java development times, it is in reality seldome that you do some coding tasks that could not have been done with public attributes instead of privates with connected getters and setters. The pythonic approach to this problem is: make everything public, and if at some point you need to encapsulate, decorate your attributes and change it into a property. Today we will work with this approach in mind.  

Learning goals
--------------
After this week you will be able to:
        
- Understand the pythonic approach to encapsulation. 
- Use public and non-public attributes in your code
- Work with properties to use encapsulation.
- And explain the pros and cons of properties and public attributes compared to Java´s private attributes with getters and setters. 

Materials
---------
* `Difference between _, __ and __xx__ in Python <https://igorsobreira.com/2010/09/16/difference-between-one-underline-and-two-underlines-in-python.html>`_
* `Python's property(): Add Managed Attributes to Your Classes <https://realpython.com/python-property/>`_
* `Notebook on properties <notebooks/OOP_Encapsulation_Propeties.rst>`_
* `Code examples from teachings <https://github.com/python-elective-kea/fall2022-code-examples-from-teachings/tree/master/ses7>`_




Exercises
---------

------------------------------------
Encaptiolation & Propeties exercises
------------------------------------

All following exercises should be done by using **Properties** when needed (Ex 1 should have also properties every where even though its not needed). The focus should be on encapsulation. 


Ex 1:  Car object
*****************

`Solution <exercises/solution/05_encapsulation/solutions.rst>`_

Create a Car class. When instanciated the object should be able to take 4 attributes (Make, Model, bhp, mph). They all 4 should be properties. (Even though this is not nessary here, you should create properties in order just to try it out).



Ex 2: Bank
**********

`Solution <exercises/solution/05_encapsulation/solutions.rst>`_

In the exercise from last monday with the bank, account and customer, change the code to use properties instead of the public variables.  

.. code:: python
   :linenos:

   class Bank:    
        def __init__(self):
           self.accounts = []

   class Account:
        def __init__(self, no, cust):
           self.no = no
           self.cust = cust

   class Customer:
        def __init__(self, name):
           self.name = name


* The bank class should futher be change into not taking any accounts as parameters at initialization. 
* The accouts should be added afterwards, eithers as a single account one at a time, or as a collection of accounts (many at the sametime).      
* Somewhere you should change the code so that a customer only can create one account.     
* The Customer class should make sure that the customer is over 18 year of age.





Ex 3: Machine -> printer
************************

`Solution <exercises/solution/05_encapsulation/solutions.rst>`_


* Create a Machine class that takes care of powering on and off a the machine.   
* Create a printer class that is a subclass of the Machine super class.   
* The printer should be able to print to console.  
* The printer should have a papertray, which should be in its own class. The papertray class should keep track of the paper, it should have the abillity to use paper and load new paper in the tray if empty.  


