---
id: classes-python
aliases:
  - classes-python
tags:
  - python
  - objects
---
## Classes
---

> [!NOTE] class
> General purpose term for custom pieces of data. Its the definition of a data type. *Class == Blueprint* of an object

##### Example of class:
---
In neighbourhoods where all houses are similar, in terms of programming we can say they were *constructed* with the same class aka they have the same blueprint. *But* those houses might have some differences such as:
- color
- people who live inside it
- furniture
- etc...

```python
# This invents a new data type
class Student:
	...

def main():
	student = get_student()
	print(f"{student.name} from {student.house}")

def get_student():
	student = Student()
	# The "." allows us to access to an attribute which is an instance variable
	student.name = input("Name: ")
	student.houde = input("House: ")
	return student

if __name__ == "__main__":
	main()

```
*attribute == instance variable*


> [!NOTE] \_\_init\_\_
> Method used to initialize an object from its class
##### How do \_\_init\_\_ work?
---
```python
class Student:
	def __init__(self, name, house)
		self.name = name
		self.house = house

def get_student():
	name = input("Name: ")
	house = input("House: ")
	return Student(name, house)
```


> [!NOTE] What is \_\_init\_\_ doing?
> It allows us to initialize an object with certain atributes aka *instance variables*
> The *self* variable allows us to access the current object who was just created
> The *Student()* function is the constructor and automatically calls the \_\_init\_\_ method



## References
---
- [[classAttributes]]