## How to Compile and Run

```bash
g++ -std=c++17 <filename>.cpp -o program
./program

```

On Windows (MinGW):

```bash
g++ -std=c++17 <filename>.cpp -o program.exe
program.exe

```

## List of Programs

| Sr. No. | File Name | Program Title | Main Concept |
| --- | --- | --- | --- |
| 1 | `FunctionOverloading.cpp` | Function Overloading | Compile-time polymorphism |
| 2 | `AreaCalculator.cpp` | Area Calculator | Function overloading with different parameters |
| 3 | `UnaryMinus.cpp` | Unary Minus Operator | Unary operator overloading |
| 4 | `PrefixPostfixIncrement.cpp` | Prefix and Postfix Increment | Unary operator overloading |
| 5 | `ComplexAddition.cpp` | Complex Number Addition | Binary `+` operator overloading |
| 6 | `DistanceComparison.cpp` | Distance Comparison | Relational operator overloading |
| 7 | `FriendOperator.cpp` | Non-member/Friend Operator | Operator overloading using a friend function |
| 8 | `BasePointerNoVirtual.cpp` | Base Pointer Without Virtual Function | Static binding demonstration |
| 9 | `BasePointerVirtual.cpp` | Base Pointer With Virtual Function | Run-time polymorphism |
| 10 | `BaseReferenceVirtual.cpp` | Base Reference With Virtual Function | Dynamic binding through references |
| 11 | `AbstractClass.cpp` | Abstract Class | Pure virtual function |
| 12 | `ShapeCollection.cpp` | Collection of Shape Pointers | Polymorphic processing |
| 13 | `VirtualDestructor.cpp` | Virtual Destructor | Safe deletion through base pointer |
| 14 | `ObjectSlicing.cpp` | Object Slicing | Why references/pointers are needed |
| 15 | `PaymentSystem.cpp` | Payment System | Abstract interface, real-world example |
| 16 | `EmployeePayroll.cpp` | Payroll Mini-Project | Integrated polymorphism application |

## Program Descriptions

1. **Function Overloading** — Defines three `add()` functions with different parameter lists to show compile-time polymorphism, where the compiler picks the correct overload.
2. **Area Calculator** — Overloads `calculateArea()` for a square, a rectangle, and a circle based on the number and type of arguments passed.
3. **Unary Minus Operator** — Overloads the unary `-` operator for a `Number` class so that `-object` returns a new object with a negated value.
4. **Prefix and Postfix Increment** — Overloads both `++object` (prefix) and `object++` (postfix) for a `Counter` class, distinguishing them with a dummy `int` parameter.
5. **Complex Number Addition** — Overloads the binary `+` operator for a `Complex` class so two complex numbers can be added using natural `+` syntax.
6. **Distance Comparison** — Overloads the `>` relational operator for a `Distance` class to compare two user-defined objects directly.
7. **Non-member/Friend Operator** — Uses a `friend` non-member function to overload `+` for expressions like `10 + complexNumber`, where the left operand isn't a class object.
8. **Base Pointer Without Virtual Function** — Shows static (compile-time) binding: calling a non-virtual function through a base pointer always invokes the base version.
9. **Base Pointer With Virtual Function** — Demonstrates run-time polymorphism: a `virtual` function called through an `Animal*` pointer correctly invokes `Dog` or `Cat` behavior.
10. **Base Reference With Virtual Function** — Passes derived `Shape` objects by base-class reference to a function, preserving virtual dispatch without copying.
11. **Abstract Class** — Defines an abstract `Shape` class with a pure virtual `area()` function that cannot be instantiated directly, only through concrete derived classes.
12. **Collection of Shape Pointers** — Stores different derived `Shape` objects (`Rectangle`, `Circle`) in a `std::vector<std::unique_ptr<Shape>>` and processes them polymorphically.
13. **Virtual Destructor** — Shows that a `virtual` destructor in the base class ensures both derived and base destructors run correctly when deleting through a base pointer.
14. **Object Slicing** — Demonstrates the object-slicing problem when a derived object is passed by value as a base type, and how pass-by-reference avoids it.
15. **Payment System** — Models a real-world abstract `Payment` interface with `CardPayment`, `UpiPayment`, and `NetBankingPayment` implementations processed polymorphically.
16. **Payroll Mini-Project** — Extends the abstract `Employee` class with `PermanentEmployee` and `ContractEmployee` to compute and print payslips using run-time polymorphism.

## Notes

* All programs are written in standard C++17 and compile without warnings using `g++ -std=c++17`.
* Each `.cpp` file contains inline comments explaining key statements and design decisions.
* Add screenshots of your compiled output (terminal or IDE) to a `screenshots/` folder if your submission requires visual proof of execution, and reference them here, e.g. `![Program 1 Output](screenshots/FunctionOverloading_output.png)`.
