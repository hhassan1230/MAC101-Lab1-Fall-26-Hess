# Lab 2: User Input and Variables

**Course:** Introduction to C++
**Due Date:** 9/28/26
**Points:** 15

## 🎯 Objective
In this lab, you will move beyond static text and create an interactive program! You will learn how to declare variables (`string` and `double`), accept input from the user using `cin`, and format dynamic output using `cout`.

## 📝 Instructions

1. **Setup your file:** Create a new C++ file named `io_lab.cpp`.
2. **Include Libraries:** You will need `<iostream>` for input/output. It is also good practice to `#include <string>` since you will be storing text.
3. **Namespace:** Add `using namespace std;` below your includes so you don't have to type `std::` before every `cin` and `cout`.
4. **The Code:** Write a program that performs the following steps inside `int main()`:
   * Declare a `string` variable called `name` and a `double` variable called `gpa`.
   * Ask the user: "What is your name?"
   * Use `cin` to store their answer in the `name` variable.
   * Greet them by name.
   * Ask the user: "What is your GPA?"
   * Use `cin` to store their answer in the `gpa` variable.
   * Print a final message using both variables, like: `Wow [name], Your GPA is [gpa] Get ya grades up!`

## 💻 Expected Output (Base Assignment)

```text
What is your name?
Sam
Hello Sam nice to meet you
What is your GPA?
2.5
Wow Sam Your GPA is 2.5 Get ya grades up!
```

---

## 🚀 Stretch Goal for Advanced Students (+5 Bonus Points)

**The "Space" Bug and Formatting**

If you run the base code and type a first *and* last name (e.g., "Sam Smith"), the program will break! This happens because standard `cin >>` stops reading text as soon as it hits a space. It will try to store "Smith" inside your `gpa` variable, causing an error. 

For bonus points, fix this bug and polish your output:

1. **Get the Full Name:** Research and use the `getline()` function instead of standard `cin >>` to safely capture a full name with spaces.
2. **Format the GPA:** Include the `<iomanip>` library and use `fixed` and `setprecision()` so that the GPA *always* prints with exactly one decimal place, even if they enter a whole number (e.g., if they enter `3`, it should print `3.0`).

**Expected Stretch Goal Output:**
```text
What is your name?
Sam Smith
Hello Sam Smith nice to meet you
What is your GPA?
3
Wow Sam Smith Your GPA is 3.0 Get ya grades up!
```

## 📤 Submission Guidelines
Upload your `io_lab.cpp` file to the course portal. If you attempted the stretch goal, please leave a comment `// Stretch goal attempted` at the very top of your file!
