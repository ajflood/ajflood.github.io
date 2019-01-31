# Sphinx Auto documentation  
[Sphinx Offical Documentation](http://www.sphinx-doc.org/en/master/index.html)

## Setup 

* Within the conf.py add any imports that need not be documented into: `autodoc_mock_imports = ["SomeModule"]`
* To auto use import the docs add the following to the index.rst: 
```
.. automodule:: ModuleToDocument
   :members:
```


##  General Use

* Within the docstring of the function or class 
```
"""Some short description of the thingy

A longer description of what this thing does.

	:param type name: Short description
	:return: Description of what is returned
	
	.. attribute:: some_class_attribute
		
		Whatever description you want to add for this attribute
		
```
* To-do's
```
.. todo::
	* First to do
	* Another to do
```


