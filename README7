# Object-Oriented Programming (OOP) in Python

## 1. Classes and Objects
Classes define blueprints for objects, and objects are instances of classes.

```python
class Car:
    def __init__(self, brand, model):
        self.brand = brand
        self.model = model

    def display_info(self):
        print(f"Car: {self.brand} {self.model}")

my_car = Car("Toyota", "Corolla")
my_car.display_info()
```

**Output:**
```
Car: Toyota Corolla
```

---

## 2. Inheritance
Inheritance allows a class to inherit attributes and methods from another class.

```python
class Vehicle:
    def __init__(self, brand):
        self.brand = brand
    
    def start_engine(self):
        print(f"{self.brand} engine started")

class Car(Vehicle):
    def __init__(self, brand, model):
        super().__init__(brand)
        self.model = model

my_car = Car("Honda", "Civic")
my_car.start_engine()
```

**Output:**
```
Honda engine started
```

---

## 3. Polymorphism
Polymorphism allows different classes to be treated as instances of the same class through a shared interface.

```python
class Dog:
    def speak(self):
        return "Woof!"

class Cat:
    def speak(self):
        return "Meow!"

def animal_sound(animal):
    print(animal.speak())

dog = Dog()
cat = Cat()
animal_sound(dog)
animal_sound(cat)
```

**Output:**
```
Woof!
Meow!
```

---

## 4. Encapsulation
Encapsulation restricts access to certain details of an object, protecting its integrity.

```python
class BankAccount:
    def __init__(self, balance):
        self.__balance = balance  # Private attribute
    
    def deposit(self, amount):
        self.__balance += amount
    
    def get_balance(self):
        return self.__balance

account = BankAccount(1000)
account.deposit(500)
print(account.get_balance())
```

**Output:**
```
1500
```

---

## 5. Abstraction
Abstraction hides implementation details and only exposes essential functionalities.

```python
from abc import ABC, abstractmethod

class Animal(ABC):
    @abstractmethod
    def make_sound(self):
        pass

class Dog(Animal):
    def make_sound(self):
        return "Bark!"

dog = Dog()
print(dog.make_sound())
```

**Output:**
```
Bark!
```

---

