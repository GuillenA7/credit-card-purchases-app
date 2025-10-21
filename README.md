# 💳 Credit Card Purchase App – Java Collections Challenge

This project was developed as part of the **[Alura](https://www.aluracursos.com/)** [ONE](https://www.oracle.com/mx/education/oracle-next-education/) program – **Java: Working with Lists and Data Collections** course.

It simulates a simple **credit card system** where users can make purchases, manage their available balance, and view a sorted summary of all transactions.

---

## 🧠 Project Overview

The application is a console-based Java program that allows users to:

* Set an initial **credit card limit**.
* Perform multiple purchases, each with a **description** and **amount**.
* Automatically **deduct** the value of purchases from the remaining balance.
* Display a **summary of all purchases**, sorted in ascending order by value.
* Stop buying either manually or when the available balance runs out.

This project reinforces key Java concepts, especially around **collections, sorting, encapsulation, and control flow**.

---

## 🧩 Class Structure

```
src/
│
├── Compra.java
├── TarjetaDeCredito.java
└── Principal.java
```

### 📄 Key Classes

* **`Compra`** – Represents a single purchase, with a description and value.
  Implements the `Comparable` interface to enable sorting by value.

* **`TarjetaDeCredito`** – Represents a credit card.
  Manages the limit, current balance, and list of purchases.
  Includes a method `lanzarCompra()` that validates whether a purchase can be made based on the remaining balance.

* **`Principal`** – Main class containing the interactive menu.
  Handles user input, purchase creation, and displays the final sorted list of purchases and remaining balance.

---

## ⚙️ Features Implemented

* Initialize a credit card with a user-defined limit.
* Add purchases with description and value.
* Automatically validate available balance before approving a purchase.
* Maintain a list of all purchases made.
* Sort purchases by value using `Comparable` and `Collections.sort()`.
* Display the final summary neatly formatted in the console.

---

## 🧪 Example Run

```
Escriba el límite de la tarjeta:
1000
Escriba la descripción de la compra:
videojuego
Escriba el valor de la compra:
500
Compra realizada!
Escriba 0 para salir o 1 para continuar
1
Escriba la descripción de la compra:
sombrero
Escriba el valor de la compra:
100
Compra realizada!
Escriba 0 para salir o 1 para continuar
0

***********************
COMPRAS REALIZADAS:

sombrero - 100.0
videojuego - 500.0

***********************
Saldo de la tarjeta: 400.0
```

---

## 🛠️ Technologies Used

* **Java 17+**
* **IntelliJ IDEA**
* **Collections Framework (`ArrayList`, `Collections.sort`)**
* **Scanner for console input**

---

## 📚 Learning Objectives

Through this challenge, you’ll practice:

* Using the **Collections Framework** (`List`, `ArrayList`).
* Implementing **interfaces** (`Comparable`).
* Managing **data sorting and ordering** in Java.
* Applying **object-oriented design principles**:

  * Encapsulation
  * Constructors and attribute initialization
  * Object interaction through methods

---

## 👩‍💻 Author

**Bruno Darío Fernández Ellerbach (Instructor: [Alura](https://www.aluracursos.com/) [ONE](https://www.oracle.com/mx/education/oracle-next-education/) Program)**

Adapted and practiced by *Jose Adrian Guillen Lamas* as part of the

**Java Object-Oriented Programming G9 – ONE** training.

---

## 📜 License

This project is for educational purposes only, as part of the Alura ONE learning path.

Feel free to clone, modify, and extend it to continue practicing your Java skills.

---

⭐ *“Practice is the best teacher — keep coding, testing, and improving.”*
