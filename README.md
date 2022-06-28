# Mocking 

![](https://miro.medium.com/max/1400/1*cfrpx1gzp5ZfgU1vqIGZEw.png)  
  

Mocking a library for testing in Python. It allows you to `replace parts` of your system under test with `mock objects` and make assertions about how they have been used.
Good explanation [here](https://youtu.be/_OyuFg9pGQg)


- Form of stubbing objects
- i.e. stub an external API to simulate outages

It gathers data on 

- If you called a method
- How you called the method
- How often you called the method

```sh
pip install mock
```


unittest.mock used to imitate objects  

## patch   
  
Replaces the real objects in the code with Mock instances.  


`patch()` can be used as decorator or context manager (for scope)  
  
After scope exit - returns function to original self.  
  


 ## USAGE 


```python
from unittest.mock import Mock
mock = Mock()
print(mock) # prints ID

# Pass mock as an argument to do_something()
myDefinedFunction(mock)

# Patch the json library
json = mock
```  
  
- Mock 
