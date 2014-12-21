Tool for creating python classes and serializing them quickly into json

Tested in python 2.7, not sure if it's 3.0 compatable.


### RUNNING ###

python generator.py
OR
./generator.py




### ADDING CLASSES ###

- Create the class in 'Types', ensure this is at the top of the file:

```
#!/usr/bin/python

from base import Base

class TestClass(Base):
	def __init__(self, classTypes, classInstances):
		Base.__init__(self, classTypes, classInstances)
	
		## your defines go below
		... now add class members
```

- To add a relation to an existing class use the generateRelation. 
   Take a look at relationTest.py for an example


- In 'generator.py' update includeTypes to include the file name 
   and class name

