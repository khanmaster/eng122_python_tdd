
- create a file called test_cases_cacl
```python
from calc import SimpleCalc
import unittest
import pytest

class Caltests(unittest.TestCase):
    calc_obj = SimpleCalc()

    def test_add(self):
        self.assertEqual(self.calc_obj.add(2, 4), 6)

    def test_subtract(self):
        self.assertEqual(self.calc_obj.subtract(4, 2), 2)

    def test_multiply(self):
        self.assertEqual(self.calc_obj.multiply(2, 3), 6)

    def test_divide(self):
        self.assertEqual(self.calc_obj.divide(6, 3), 2)

```
- run `python -m pytest -v`
### refector code to pass tests
```python
class SimpleCalc:

    def add(self, value1, value2):
        return value1 + value2

    def subtract(self, value1, value2):
        return value1 - value2

    def multiply(self, value1, value2):
        return value1 * value2

    def divide(self, value1, value2):
        return value1 / value2
    
    # create a function for DOB - another function for % 
    # another function for cm to m
    # 
```

