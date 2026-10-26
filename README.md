# Experiment No. 2

## Title: Programs on Method and Constructor Overloading

## 1. Program Code

### A. Method Overloading

**File Name: Main.java**

```java
class Calculator {

    // Method with 2 integer parameters
    int add(int a, int b) {
        return a + b;
    }

    // Method with 3 integer parameters
    int add(int a, int b, int c) {
        return a + b + c;
    }

    // Method with 2 double parameters
    double add(double a, double b) {
        return a + b;
    }
}

public class Main {
    public static void main(String[] args) {

        Calculator calc = new Calculator();

        System.out.println("Sum (int, int): "
                + calc.add(10, 20));

        System.out.println("Sum (int, int, int): "
                + calc.add(10, 20, 30));

        System.out.println("Sum (double, double): "
                + calc.add(10.5, 20.5));
    }
}
```

### Output

```text
Sum (int, int): 30
Sum (int, int, int): 60
Sum (double, double): 31.0
```

---

### B. Constructor Overloading

**File Name: Main.java**

```java
class Student {
    int id;
    String name;

    // Default constructor
    Student() {
        id = 0;
        name = "Unknown";
    }

    // Constructor with one parameter
    Student(int id) {
        this.id = id;
        name = "Not Specified";
    }

    // Constructor with two parameters
    Student(int id, String name) {
        this.id = id;
        this.name = name;
    }

    void display() {
        System.out.println("ID: " + id
                + ", Name: " + name);
    }
}

public class Main {
    public static void main(String[] args) {

        Student s1 = new Student();
        Student s2 = new Student(101);
        Student s3 = new Student(102, "Amit");

        s1.display();
        s2.display();
        s3.display();
    }
}
```

### Output

```text
ID: 0, Name: Unknown
ID: 101, Name: Not Specified
ID: 102, Name: Amit
```

## 2. Aim

To write Java programs demonstrating method overloading and constructor overloading.

## 3. Theory

- **Method Overloading:** Defining multiple methods with the same name but different parameters.
- **Constructor:** A special method used to initialize an object.
- **Constructor Overloading:** Defining multiple constructors with different parameters.
- **Compile-Time Polymorphism:** Method overloading is an example of compile-time polymorphism.
- **this Keyword:** Refers to the current object.

## 4. Conclusion

Thus, Java programs demonstrating method overloading and constructor overloading were successfully implemented.

Both concepts allow the use of the same name with different parameter lists.
