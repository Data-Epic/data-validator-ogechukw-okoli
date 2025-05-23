# **dataverifier**

## **Overview**
dataverifier is a Python package designed to efficiently validate various types of personal data, including:
- **Email addresses**
- **Phone numbers**
- **Dates**
- **URLs**

This package follows **Object-Oriented Programming (OOP)** principles, ensuring modularity, reusability, and easy integration into different projects.

---

## **Installation**
Install the package using:

pip install dataverifier
```

---

## **Usage**

### **1 Import the Validator Class**
```python
from dataverifier.validator import DATAVALIDATOR
```

### **2 Validate an Email**
```python
data = "example@gmail.com"
validator = DATAVALIDATOR(data)
print(validator.validate_email())  # Output: True
```

### **3 Validate a Phone Number**
```python
data = "+1-832-005-3034"
validator = DATAVALIDATOR(data)
print(validator.validate_phone()) # Output: True
To check if a number if from a particular contitnent , you can do this

data = "+234901245890"
validator = DATAVALIDATOR(data)
print(validator.african_numbers()) #output :True
repeat for other continents by simply calling the method continentname_numbers()
```

### **4 Validate a Date**
```python
data = "2024-02-1123"
validator = DATAVALIDATOR(data)
print(validator.validate_date())  # Output: False
```

### **5 Validate a URL**
```python
data = "https://google.com"
validator = DATAVALIDATOR(data)
print(validator.validate_url())  # Output: True
```

---

## **Running Tests**
The package includes unit tests to ensure proper functionality. Run tests using:
```bash
pytest-v
```

---

## **Contributing**
Contributions are welcome! To contribute:
1. **Fork** the repository
2. **Create** a feature branch:
   ```bash
   git checkout -b featurebranch
   ```
3. **Commit** your changes:
   ```bash
   git commit -m "Added new feature"
   ```
4. **Push** to the branch:
   ```bash
   git push origin featurebranch
   ```
5. **Open a Pull Request**

---

## **License**
This project is licensed under the **MIT License**.

---

## **Author**
**OKOLI OGECHUKWU ABIMBOLA**
Email: okoliogechi74@gmail.com