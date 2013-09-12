This is my hacked version of `zope.testrunner`_.
It essentially just adds an option: --rerun
This enables one to change code and rerun the same test without
having to load all other layers each time.

For example ::

    bin/test -s my.egg -t test_bar --rerun
    
    
Requires zc.recipe.testrunner = 2.0.0


Known Issues
=============

* **sqlalchemy** 
    I have had issues with testing methods that use sqlalchemy

.. _zope.testrunner: http://docs.zope.org/zope.testrunner/
