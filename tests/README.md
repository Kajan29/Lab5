# Tests

This folder contains test files to verify your solutions.

## 🧪 Purpose

- **Unit Tests**: Test individual functions/methods
- **Integration Tests**: Test complete workflows
- **Test Cases**: Verify expected outputs for given inputs

## 📝 Naming Convention

Use `test_` prefix for test files:
- `test_exercise1.py` - Tests for Exercise 1
- `test_exercise2.py` - Tests for Exercise 2
- `test_exercise3.py` - Tests for Exercise 3

## 🔧 Testing Frameworks

### Python - unittest or pytest
```python
import unittest
from src.exercise1.main import function_name

class TestExercise1(unittest.TestCase):
    def test_basic_case(self):
        result = function_name(input)
        self.assertEqual(result, expected_output)
```

### Java - JUnit
```java
import org.junit.Test;
import static org.junit.Assert.*;

public class TestExercise1 {
    @Test
    public void testBasicCase() {
        // Your test code here
    }
}
```

## 🚀 Running Tests

### Python
```bash
# Using unittest
python -m unittest discover tests

# Using pytest (if installed)
pytest tests/
```

### Java
```bash
# Compile and run with JUnit
javac -cp .:junit.jar tests/TestExercise1.java
java -cp .:junit.jar org.junit.runner.JUnitCore TestExercise1
```

## ✅ Test Checklist

For each exercise, create tests for:
- [ ] Normal/typical inputs
- [ ] Edge cases (empty, zero, maximum values)
- [ ] Invalid inputs (if applicable)
- [ ] Boundary conditions
- [ ] Expected outputs match requirements

## 📊 Example Test Structure

```
tests/
├── test_exercise1.py    # Exercise 1 tests
├── test_exercise2.py    # Exercise 2 tests
├── test_exercise3.py    # Exercise 3 tests
└── README.md            # This file
```
