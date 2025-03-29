#  Fraction Arithmetic in Python – Simplified!

# 🔍 Why Can’t Python Handle Fractions Like Integers?

That’s the question I asked myself before building a Fraction class that makes fraction operations intuitive. With operator overloading, now Fraction(3,4) + Fraction(2,5) works naturally.

This project helped me dive deeper into Encapsulation, Polymorphism, and Dunder Methods. 

# Check out my implementation! 🚀

✨ Bringing Fractions to Life with Python! 🧮🐍

Ever tried working with fractions in Python and wished they behaved like regular numbers? 🤔 Well, I decided to build a Fraction class that supports addition, subtraction, multiplication, and division using operator overloading!🚀

✨ This project showcases Object-Oriented Programming (OOP) principles like Encapsulation, Abstraction, and Polymorphism, making fraction calculations intuitive and Pythonic.



✅ Supports arithmetic operations with +, -, *, and /

✅ Uses dunder methods (__add__, __sub__, __mul__, __truediv__) for natural interactions.

✅ Implements Encapsulation to store and manipulate fraction data effectively.

✅ Operator Overloading for mathematical operations on fractions.



# How It Works

1️⃣ Creating a Fraction Object

We define a fraction as Fraction(numerator, denominator).

x = Fraction(3, 4)  # Represents 3/4

y = Fraction(2, 5)  # Represents 2/5

2️⃣ Addition (+ Operator Overload) --> Adding two fractions

def __add__(self, other):

    temp_num = self.num * other.den + other.num * self.den

    temp_den = self.den * other.den

    return Fraction(temp_num, temp_den)

Example Usage:

result = x + y  # (3/4 + 2/5)

print(result)   # Output: 23/20


3️⃣ Subtraction (- Operator Overload) --> Subtracting two fractions:


def __sub__(self, other):

    temp_num = self.num * other.den - other.num * self.den

    temp_den = self.den * other.den

    return Fraction(temp_num, temp_den

Example Usage:

result = x - y  # (3/4 - 2/5)

print(result)   # Output: 7/20


4️⃣ Multiplication (* Operator Overload) --> Multiplying two fractions


def __mul__(self, other):

    temp_num = self.num * other.num

    temp_den = self.den * other.den

    return Fraction(temp_num, temp_den)

Example Usage:

result = x * y  # (3/4 * 2/5)

print(result)   # Output: 6/20


5️⃣ Division (/ Operator Overload) --> Dividing two fractions


def __truediv__(self, other):

    temp_num = self.num * other.den

    temp_den = self.den * other.num

    return Fraction(temp_num, temp_den)

Example Usage:

result = x / y  # (3/4 ÷ 2/5)

print(result)   # Output: 15/8


6️⃣ String Representation (__str__) --> To neatly display the fraction

def __str__(self):

    return f"{self.num}/{self.den}"

print(x)  # Output: 3/4

# Key Takeaways 🏆

📌 Operator Overloading: Enables mathematical operations on custom objects.

 📌 Encapsulation: Ensures that fraction data is stored and manipulated securely.

 📌 Pythonic Code: Makes fraction operations intuitive and readable.

#Python #OOP #Fractions #Coding #OperatorOverloading #Programming #Encapsulation #DunderFunctions

