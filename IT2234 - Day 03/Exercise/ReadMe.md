# JavaScript Function Exercise

This repository contains four JavaScript files demonstrating different function implementations, including arrow functions, rest parameters, prime number checking, and recursion.

## Getting Started
Ensure you have Node.js installed or run the scripts in the browser console.

## Code Overview

### 1. `Arrow.js` - Arrow Functions
This script demonstrates JavaScript arrow functions.

- **Sum of two numbers:**
  ```js
  const sum = (x, y) => { return x + y };
  console.log(sum(5, 6));
  ```
  **Output:**
  ```sh
  11
  ```
  
- **Multiplication with a default parameter:**
  ```js
  const mul = (x, y = 2) => { return x * y };
  console.log(mul(5));
  ```
  **Output:**
  ```sh
  10
  ```
<img width="959" alt="Arrow" src="https://github.com/user-attachments/assets/29848ffc-7ee8-4c83-9293-76486fd75329" />

---

### 2. `Arrow-RestParameter.js` - Rest Parameter Function
This script demonstrates the use of rest parameters in functions.

- **Sum of multiple numbers using rest parameters:**
  ```js
  const FindSum = (...n) => {
      let sum = 0;
      for (let c of n) {
          sum += c;
      }
      return sum;
  };
  console.log("Sum: " + FindSum(7,8,9,4,2,5));
  ```
  **Output:**
  ```sh
  Sum: 35
  ```
<img width="959" alt="Arrow rest" src="https://github.com/user-attachments/assets/a976dc10-7c94-4f7b-879e-1edf216371b0" />

---

### 3. `PrimeChecker.js` - Prime Number Checker
This script checks whether a given number is prime.

- **Prime checking function:**
  ```js
  function isPrime(a) {
      let primeNumber = true;
      if (a == 1) {
          primeNumber = false;
      } else {
          for (let i = 2; i <= a / 2; i++) {
              if (a % i == 0) {
                  primeNumber = false;
              }
          }
      }
      return primeNumber;
  }
  ```
  
- **Usage Example:**
  ```js
  function primeChecker(a, isPrime) {
      if (isPrime) {
          console.log(a + " is a prime number");
      } else {
          console.log(a + " is not a prime number");
      }
  }
  
  primeChecker(10, isPrime(10));
  primeChecker(7, isPrime(7));
  ```
  **Output:**
  ```sh
  10 is not a prime number
  7 is a prime number
  ```
<img width="959" alt="prime checker" src="https://github.com/user-attachments/assets/ebabd973-55c5-4227-ab07-32209a62ddb3" />

---

### 4. `Recurcise.js` - Recursive Function
This script demonstrates recursion by printing numbers from 1 to `n`.

- **Recursive function:**
  ```js
  function recursive(n) {
      if (n <= 0) {
          console.log("Invalid");
          return;
      }
      recursive(n - 1);
      console.log(n);
  }
  recursive(5);
  ```
  **Output:**
  ```sh
  1
  2
  3
  4
  5
  ```
<img width="959" alt="recursive" src="https://github.com/user-attachments/assets/2c858b86-feec-4e87-b6aa-d4d10c82bc60" />


## Running the Code
To execute any of the JavaScript files:
```sh
node filename.js
```
Or, copy and paste the code into the browser's developer console.

