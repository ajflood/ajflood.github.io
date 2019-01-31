# Sphinx Auto documentation  
[Sphinx Offical Documentation](http://www.sphinx-doc.org/en/master/index.html)

## Setup 

* Within the conf.py add any imports that need not be documented into: autodoc_mock_imports = ["SomeModule"]
* To auto use import the docs add the following to the index.rst: 
```
.. automodule:: ModuleToDocument
   :members:
```


##  General Use
