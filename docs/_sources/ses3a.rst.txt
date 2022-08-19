Session 3a - Data Structures & List Comprehensions
==================================================

Today we will start by talking about your mandatory assignment from last week.   
We will then look at different kinds of data sets and determine what data structure could be used for representing this specific kind of data.    
We will also look at Pythons collection module and see how to use this on our data.     
Last we will work with list comprehensions.    


Learning goals
--------------


Materials
---------
* `collections — Container datatypes <https://docs.python.org/3/library/collections.html>`_
* `Speed of list comprehensions vs for loop <https://stackoverflow.com/questions/30245397/why-is-a-list-comprehension-so-much-faster-than-appending-to-a-list/30245465#30245465>`_


Exercises
---------

--------------
Ex1: Wordcount      
--------------
`solution <exercises/solution/03_set_dict/dicts.rst>`_

| Copy/Paste the code below into a file and call it words.py
| Do the exercises and run them.
| You can use either of these files for testing your solution.

* `small.txt <exercises/dict_exercises/count_words_in_file/small.md>`_
* `alice.txt <exercises/dict_exercises/count_words_in_file/small.md>`_    


**words.py**


.. literalinclude:: exercises/dict_exercises/count_words_in_file/words.py
   :linenos:
   :language: python






* `words.py <exercises/dict_exercises/count_words_in_file/words.py>`_
* `small.txt <exercises/dict_exercises/count_words_in_file/smalltxt>`_
* `alice.txt <exercises/dict_exercises/count_words_in_file/alice.txt>`_

-------------------------------
Ex2: Log Puzzle Python Exercise
-------------------------------
* `Log Puzzel <exercises/dict_exercises/logpuzzel/logpuzzel.md>`_


   
----------------------------
Ex1: Count letters and words
----------------------------

By importing the `collections <https://docs.python.org/3/library/collections.html#module-collections>`_ module you have access to the `Counter object <https://docs.python.org/3/library/collections.html#counter-objects>`_ .    
Use this object to count the occurrences of each words in this `text file <>`_ .    



