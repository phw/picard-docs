.. MusicBrainz Picard Documentation Project

.. _func_right:

$right
======

| Usage: **$right(text,number)**
| Category: text

**Description:**

Returns the last ``number`` characters from ``text``.  If ``number`` is less than 1, then the
value used is the number of characters in ``text`` plus ``number`` (e.g.: ``$right(abcd,0)``
is the same as ``$right(abcd,4)``).  If ``number`` is missing or a negative number greater
than the number of characters in ``text``, the function will return an empty string.


**Example:**

The following statements will return the values indicated:

.. code-block:: taggerscript

    $right(abcd,2)   ==>  "cd"
    $right(abcd,0)   ==>  "cd"
    $right(abcd,-1)  ==>  "bcd"
    $right(abcd,)    ==>  ""
    $right(abcd,-5)  ==>  ""
