Very Simple UML to Python Generator
===================================

Very simple Accelo Python generator from UML class diagram. This generator is presented as an example and can be used as work basis but, depending on your purpose, is definitively not enough.

## Sources ##
Model to text (m2t) source is located in `simple-python/codegen` folder while generator is described by `simple-python/generator.xml` file.

## UML Diagram & Translation ##
Class diagrams contained in an UML project are used for python code generation. Python compilation choices are reported in the following table.

| UML | Python  |
| :-: |:-------:|
| Package | module file|
| Class | class |
| Interface | class |
| Property | class attribute |
| Operation | class operation |
| Enumeration | class |

## Why a fork? ##
Because I need my python code generate constructor with super methods. Example:
```
class Example(Object):
    def __init__(self, *args, **kwargs):
        super(Example, self).__init__(*args, **kwargs)
```
