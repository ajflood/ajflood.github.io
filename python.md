# Python Stuff I Regularly Use

[General python functionality](python/py_general.md)
[Styling](python/py_styling.md)  
[Formatted Output](python/py_formatted_output.md)  
[Logging](python/py_logging.md)  
[Arrayfire](python/py_arrayfire.md)  
[Sphinx Auto-documentation](python/sphinx.md)

### Reading and writing to file

`file_object  = open(“filename”, “mode”)`

#### Modes
- r: Read mode which is used when the file is only being read 
- w: Write mode which is used to edit and write new information to the file (any existing files with the same name will be erased when this mode is activated) 
- a: Appending mode, which is used to add new data to the end of the file; that is new information is automatically amended to the end 
- r+: Special read and write mode, which is used to handle both actions when working with a file 

#### Writing to file

`file_object.write("Some thing to be written to file")`


