<img src="./resources/images/banner.jpg" alt="banner" width="450" height="230" style="display: block; margin: 0 auto" />

---

## Motivation

The intent behind the creation of this repository is to document my learning as I try to develop a reasonable understanding about design patterns for software development. And since that is the case, I am unable to assure the total correctness of all the content written.

This repository is _**open for contributions**_.

---

## Object Oriented Programming (OOP) - Basics

Programming paradigm which focuses on the organization of the software into reusable pieces of code called _`classes`_, based on the grouping of related data and behaviors. Theses classes can be thought of as general blueprints or recipes that define the structure for _`objects`_. Objects are concrete instances of classes.

In the UML diagram below, we have a very basic `Person` class which contains a few private attributes and public methods:

![OOP_class_example_1](resources/uml/oop_class_1.png)

Below is a C++ implementation of this class:

```cpp
class Person {
  private:
    string name;
    string country;
    string occupation;
    int age;
  public:
    Person(string name, string country, string occupation, int age)
      : name{name}, country{country}, occupation{occupation}, age{age} {}

    string getName(){
      return this->name;
    }
    string getNationality(){
      return this->country;
    }
    void changeJob(const string &newJob){
      this->occupation = newJob;
    }
    ...
}
```

### Abstraction

### Encapsulation

### Inheritance

### Polymorphism

---

## - **SOLID Principles**

### >> **S**ingle Responsibility Principle [SRU]

### >> **O**pen/Closed Principle [OCP]

### >> **L**iskov Substitution Principle

### >> **I**nterface Segregation Principle

### >> **D**ependency Inversion

---

## - **Creational Design Patterns**

### >> Factory

### >> Abstract Factory

### >> Builder

### >> Prototype

### >> Singleton

---

## - **Structural Design Patterns**

### >> Adapter

### >> Bridge

### >> Composite

### >> Decorator

### >> Facade

### >> Flyweight

### >> Proxy

---

## - **Behavioral Design Patters**

### >> Chain of Responsibility

### >> Command

### >> Iterator

### >> Mediator

### >> Memento

### >> Observer

### >> State

### >> Strategy

### >> Template Method

### >> Visitor

---

## References

- [Dive Into Design Patterns by Alexander Shvets](https://refactoring.guru/design-patterns/book)
- Clean Architecture by Robert C. Martin
- [Design Patterns in Modern C++ by Dmitri Nesteruk](https://www.udemy.com/course/patterns-cplusplus/)
