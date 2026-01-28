# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Babel](https://babeljs.io/) (or [oxc](https://oxc.rs) when used in [rolldown-vite](https://vite.dev/guide/rolldown)) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## React Compiler

The React Compiler is not enabled on this template because of its impact on dev & build performances. To add it, see [this documentation](https://react.dev/learn/react-compiler/installation).

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.


ASSIGNMENT WORK OF INTERNSHIP.

1.Differnce between HTTP and HTTPS.
A.) HTTP and HTTPS are both protocols for loading web pages, but HTTPS adds encryption and identity verification to make communication secure.
	HTTP	HTTPS
Definition	HTTP (Hypertext Transfer Protocol): Rules for how browsers and servers send and receive web data in plain text.
	HTTPS (Hypertext Transfer Protocol Secure): HTTP plus an encryption layer (SSL/TLS) so data is sent securely.
Security	HTTP sends data as readable plain text, so attackers can intercept or modify it.
	HTTPS encrypts data using SSL/TLS, protecting it from eavesdropping and tampering.

Identity/Trust	HTTP does not verify the server’s identity.	HTTPS uses digital certificates to verify the server, giving the padlock icon and “https://” in the address bar
Ports & URL’S	HTTP usually uses port 80 and URLs start with http://.	HTTPS usually uses port 443 and URLs start with https://.
Typical usage	HTTP may be used for non-sensitive, internal, or legacy content (though less common now).	HTTPS is recommended for almost all sites, especially for logins, payments, and any user data.


2.) Define Web Architecture  &DNS.
A.) Web architecture refers to the high-level structure and organization of the World Wide Web as a whole, including how core components like browsers, web servers, DNS systems, HTTP/HTTPS protocols, and content delivery networks interact globally to deliver web content to users.
DNS (Domain Name System) is the internet's phonebook that translates human-readable domain names (like google.com) into machine-readable IP addresses (like 142.250.190.78) so browsers can locate and connect to web servers.

3.) Difference between ARIA & WAI ARIA.
A.)
Aspect	ARIA	WAI-ARIA
Full Name	Accessible Rich Internet Applications	Web Accessibility Initiative - Accessible Rich Internet Applications
Definition	Technical specification (attributes like role, aria-label)	W3C initiative/framework that includes the ARIA specification
Scope	HTML attributes for roles, states, properties	Complete WAI standards suite (ARIA + practices, authoring guidelines)
Usage	<div role="button" aria-label="Close">X</div>	The umbrella term covering ARIA 1.0, 1.1, 1.2 specs
Relationship	Part of WAI-ARIA	Contains ARIA + additional docs (Core AAM, HTML-AAM)
Example	aria-hidden="true" attribute	WAI-ARIA 1.2 specification document
Simple rule: ARIA = the code attributes you write. WAI-ARIA = the complete W3C standard (including ARIA)

4.) How Arithmetic & Concatenation operators work in browser.
A.)
Arithmetic operator :In browsers work through the JavaScript engine (V8 in Chrome, Spider Monkey in Firefox) following ECMAScript standards. They perform math on numbers with automatic type conversion.
How browsers execute arithmetic
•	Type coercion: Strings convert to numbers automatically (except for + with strings).
2. NaN handling: Invalid math returns NaN.
3. Floating point precision: Uses IEEE 754 double precision.

concatenation in browsers uses the + operator, which automatically triggers when any operand is a string. Unlike other arithmetic operators, + prioritizes string joining over numeric addition.
How browsers handle concatenation
Core rule: If either side of + is a string → concatenation. Otherwise → arithmetic.

5.) Programs on if, else, else if, switch, looping conditions and execute 7 programs on each condition (eg if condition 7 programs).

A.)
1. IF,  IF-ELSE and ELSE-IF.
Code-1. AGE
let age = 17;
if (age >= 18) {
    console.log("✅ Eligible to vote");
} else {
    console.log("❌ Not eligible to vote");
}
// Output: ❌ Not eligible to vote 

CODE-2.Even/Odd checker.
let number = 42;
if (number % 2 === 0) {
    console.log(number + " is EVEN");
} else {
    console.log(number + " is ODD");
}
// Output: 42 is EVEN 

CODE-3. Traffic Light System.
let light = "yellow";
if (light === "green") {
    console.log("🚦 GO");
} else if (light === "yellow") {
    console.log("⚠️ SLOW DOWN");
} else if (light === "red") {
    console.log("🛑 STOP");
} else {
    console.log("❓ Invalid light");
}
// Output: ⚠️ SLOW DOWN 

CODE-4.Student Grade calculator.

let marks = 78;
if (marks >= 90) {
    console.log("Grade: A+ 🎉");
} else if (marks >= 80) {
    console.log("Grade: A 👍");
} else if (marks >= 70) {
    console.log("Grade: B 👌");
} else if (marks >= 60) {
    console.log("Grade: C 😐");
} else if (marks >= 50) {
    console.log("Grade: D ⚠️");
} else {
    console.log("Grade: F ❌");
}
// Output: Grade: B 

CODE-5.Leap year Detector.
let year = 2020;
if ((year % 4 === 0 && year % 100 !== 0) || (year % 400 === 0)) {
    console.log(year + " is a LEAP YEAR ✅");
} else {
    console.log(year + " is NOT a leap year ❌");
}
// Output: 2020 is a LEAP YEAR ✅

CODE-6.Atm Balance Check.
let balance = 500;
let withdraw = 700;
if (balance >= withdraw) {
    console.log("✅ Withdrawal successful");
    console.log("New balance: $" + (balance - withdraw));
} else {
    console.log("❌ Insufficient balance");
    console.log("Current balance: $" + balance);
}
// Output: ❌ Insufficient balance

CODE-7.Weather Outfit Suggester.
let temp = 25;
if (temp >= 30) {
    console.log("👕 T-shirt & shorts");
} else if (temp >= 20) {
    console.log("👔 Shirt & jeans");
} else if (temp >= 10) {
    console.log("🧥 Jacket required");
} else {
    console.log("🧤❄️ Winter clothing");
}
// Output: 👔 Shirt & jeans.

2.SWITCH.
CODE-1.Weekday Names.
let day = 3; // 1=Mon, 7=Sun
switch(day) {
    case 1: console.log("Monday 💼"); break;
    case 2: console.log("Tuesday 📅"); break;
    case 3: console.log("Wednesday 🗓️"); break;
    case 4: console.log("Thursday ⏰"); break;
    case 5: console.log("Friday 🎉"); break;
    case 6: console.log("Saturday 🏖️"); break;
    case 7: console.log("Sunday 😴"); break;
    default: console.log("Invalid day");
}
// Output: Wednesday 🗓️.

CODE-2.Simple Calculator.
let num1 = 12, num2 = 4, operator = '*';
let result;
switch(operator) {
    case '+': result = num1 + num2; break;
    case '-': result = num1 - num2; break;
    case '*': result = num1 * num2; break;
    case '/': result = num1 / num2; break;
    case '%': result = num1 % num2; break;
    default: result = "Invalid operator";
}
console.log(`${num1} ${operator} ${num2} = ${result}`);
// Output: 12 * 4 = 48 

CODE-3.Traffic Light Controller.
let signal = "green";
switch(signal) {
    case "red":   console.log("🛑 STOP"); break;
    case "yellow": console.log("⚠️ PREPARE TO STOP"); break;
    case "green":  console.log("✅ GO"); break;
    default: console.log("❌ Invalid signal");
}
// Output: ✅ GO 

CODE-4.Student Grade System.

let marks = 82;
switch(true) {
    case marks >= 90: console.log("A+ 🥇"); break;
    case marks >= 80: console.log("A 👍"); break;
    case marks >= 70: console.log("B 👌"); break;
    case marks >= 60: console.log("C 😐"); break;
    case marks >= 50: console.log("D ⚠️"); break;
    default: console.log("F ❌");
}
// Output: A 👍
CODE-5.Month Days Counter.
let month = 2;
switch(month) {
    case 1: case 3: case 5: case 7: 
    case 8: case 10: case 12: 
        console.log("31 days 📅"); break;
    case 4: case 6: case 9: case 11:
        console.log("30 days 📆"); break;
    case 2: console.log("28/29 days (Feb) ❄️"); break;
    default: console.log("Invalid month");
}
// Output: 28/29 days (Feb) 

CODE-6.Vowel Identifier.
let char = 'E';
switch(char.toUpperCase()) {
    case 'A': case 'E': case 'I': 
    case 'O': case 'U': 
        console.log(`${char} is VOWEL 🔊`); break;
    default: console.log(`${char} is CONSONANT 📝`);
}
// Output: E is VOWEL.
CODE-7.Shopping Discount Calculator.
let totalBill = 850;
switch(true) {
    case totalBill >= 1000: console.log("10% OFF = ₹" + (totalBill * 0.1)); break;
    case totalBill >= 700:  console.log("7% OFF = ₹" + (totalBill * 0.07)); break;
    case totalBill >= 500:  console.log("5% OFF = ₹" + (totalBill * 0.05)); break;
    default: console.log("No discount 😔");
}
// Output: 7% OFF = ₹59.5

3.Looping Conditions
a. For Loop
CODE-1.Print Number 1- 10.
console.log("=== 1 to 10 ===");
for(let i = 1; i <= 10; i++) {
    console.log(i);
}
// Output: 1,2,3,...,10 

CODE-2.Sum of First 10 Numbers.
let sum = 0;
for(let i = 1; i <= 10; i++) {
    sum += i;
}
console.log("Sum 1-10 =", sum); 
//output:  55

 CODE-3.Even Numbers 0-20.
console.log("=== Even Numbers ===");
for(let i = 0; i <= 20; i += 2) {
    console.log(i);
}
// Output: 0,2,4,...,20 

CODE-4.Array Iteration (Fruits).
const fruits = ["Apple", "Banana", "Cherry", "Date"];
console.log("=== Fruits List ===");
for(let i = 0; i < fruits.length; i++) {
    console.log(`${i+1}. ${fruits[i]}`);
}
// Output: 1. Apple, 2. Banana...

CODE-5. Multiplication Tables.
let tableNum = 7;
console.log(`=== ${tableNum} Table ===`);
for(let i = 1; i <= 10; i++) {
    console.log(`${tableNum} × ${i} = ${tableNum * i}`);
}
// Output: 7 × 1 = 7, 7 × 2 = 14... 

CODE-6.Reverse Countdown.
console.log("=== Countdown 10-1 ===");
for(let i = 10; i >= 1; i--) {
    console.log(i);
}
console.log("Liftoff! 🚀");
// Output: 10,9,...,1,Liftoff! 

CODE-7.Pattern Printing(Stars).
console.log("=== Star Pattern ===");
for(let i = 1; i <= 5; i++) {
    let stars = "*".repeat(i);
    console.log(stars);
}
// Output:
// *
// **
// ***
// ****
// ***** 

b. While Loop
CODE-1.Countdown Timer.
let countdown = 10;
console.log("=== Launch Countdown ===");
while(countdown > 0) {
    console.log(countdown + "...");
    countdown--;
}
console.log("🚀 LIFTOFF!");
// Output: 10...9...8...1... LIFTOFF! 
CODE-1.Sum Positive Numbers.
let num = 0, total = 0;
console.log("=== Sum Positives ===");
while(num >= 0) {
    total += num;
    num = parseInt(prompt("Enter number (negative to stop):")) || 0;
}
console.log("Total sum:", total);
// Enter: 5,3,2,-1 → Total sum: 10
CODE-3.Factorial Calculator.
let n = 5, factorial = 1;
console.log(`=== ${n}! Calculation ===`);
let i = 1;
while(i <= n) {
    factorial *= i;
    console.log(`${i} × ${factorial}`);
    i++;
}
console.log(`${n}! = ${factorial}`); // 120 
CODE- 4: Array Traversal.
const students = ["Alice", "Bob", "Charlie", "Diana"];
let index = 0;
console.log("=== Student Roll Call ===");
while(index < students.length) {
    console.log(`${index + 1}. ${students[index]}`);
    index++;
}
// Output: 1. Alice, 2. Bob... 
CODE- 5: Guessing Game.
let secret = 7, guess = 0, attempts = 0;
console.log("=== Guess the number (1-10) ===");
while(guess !== secret && attempts < 3) {
    guess = parseInt(prompt("Guess:")) || 0;
    attempts++;
    if(guess < secret) console.log("Higher!");
    else if(guess > secret) console.log("Lower!");
}
if(guess === secret) console.log("✅ Correct!");
else console.log("❌ Game Over");
// Tests number guessing 
CODE-6.Reverse Number Printing.
let start = 50;
console.log("=== Numbers 50→1 (step -5) ===");
while(start >= 1) {
    console.log(start);
    start -= 5;
}
// Output: 50,45,40,...,5 
CODE-7.Password Validator.
let password = "", maxTries = 3, tries = 0;
let correctPass = "secret123";
console.log("=== Login System ===");
while(password !== correctPass && tries < maxTries) {
    password = prompt("Enter password:");
    tries++;
    if(password !== correctPass) {
        console.log(`❌ Wrong! ${maxTries - tries} tries left`);
    }
}
if(password === correctPass) {
    console.log("✅ Access Granted!");
} else {
    console.log("🚫 Account Locked");
}
// Enter: wrong, wrong, secret123

c. Do-While Loop
CODE-1. Menu System (Runs Once Minimum).
let choice = "";
console.log("=== Restaurant Menu ===");
do {
    console.log("\n1. Pizza  2. Burger  3. Exit");
    choice = prompt("Choose (1-3):") || "0";
    switch(choice) {
        case "1": console.log("🍕 Pizza ordered!"); break;
        case "2": console.log("🍔 Burger ordered!"); break;
        case "3": console.log("👋 Goodbye!"); break;
        default: console.log("❌ Invalid choice");
    }
} while(choice !== "3");
// Enter: 1,2,3 → Orders + Goodbye 
CODE-2.Password Login (At Least 1 Try).
let password = "", tries = 0, maxTries = 3;
let correct = "admin123";
console.log("=== Secure Login ===");
do {
    password = prompt("Enter password:") || "";
    tries++;
    if(password !== correct) {
        console.log(`❌ Wrong! ${maxTries - tries} tries left`);
    }
} while(password !== correct && tries < maxTries);
if(password === correct) {
    console.log("✅ Login Successful!");
} else {
    console.log("🚫 Account Locked!");
}
// Tests even if first try fails
CODE-3. Numbers 1-5 (Classic Example).
let i = 1;
console.log("=== 1 to 5 (do-while) ===");
do {
    console.log(i);
    i++;
} while(i <= 5);
// Output: 1,2,3,4,5 [web:233]
CODE-4.ATM Withdrawal (Minimum Display).
let balance = 1000, amount = 0;
console.log("=== ATM ===");
do {
    console.log(`Balance: ₹${balance}`);
    amount = parseInt(prompt("Withdraw (0=exit):")) || 0;
    if(amount > 0 && amount <= balance) {
        balance -= amount;
        console.log(`✅ Withdrew ₹${amount}`);
    } else if(amount > balance) {
        console.log("❌ Insufficient funds");
    }
} while(amount !== 0);
// Shows balance first, then loops
CODE-5. Dice Roll Until 6.
let roll, rolls = 0;
console.log("=== Roll until 6 ===");
do {
    roll = Math.floor(Math.random() * 6) + 1;
    rolls++;
    console.log(`Roll ${rolls}: ${roll}`);
} while(roll !== 6);
console.log(`🎉 Got 6 in ${rolls} rolls!`);
// Always rolls at least once
CODE-6.Countdown (Even if 0).
let count = 0;
console.log("=== Special Countdown ===");
do {
    console.log("T-minus " + count + "...");
    count++;
} while(count < 3);
// Runs even when count=0 initially 
CODE-7. Shopping Cart (Add Items).
console.log("=== Shopping Cart ===");
do {
    item = prompt("Add item (or 'done'):") || "";
    if(item !== "done" && item !== "") {
        cart.push(item);
        console.log(`✅ Added: ${item}`);
    }
} while(item !== "done");
console.log("Final cart:", cart.join(", "));
// Always prompts first 

4. Assignment
1) Execute do-while, Math object, function structure execution
A do-while loop executes the code at least once before checking the condition.
It is useful when the loop must run minimum one time.
The Math object provides built-in functions like Math.sqrt(), Math.random(), Math.max().
A function is a reusable block of code defined using function keyword.
Function execution happens when the function is called.
These concepts help in looping, calculations, and modular programming.

5. Assignment
1) Create an array in all ways & work through all loops
let a = [1, 2, 3];
let b = new Array(4, 5, 6);
let c = [];
c[0] = 7;

for (let i = 0; i < a.length; i++) console.log(a[i]);
for (let x of b) console.log(x);
for (let i in c) console.log(c[i]);


Arrays can be created using literals, constructor, or index assignment.
Loops like for, for...of, and for...in are used to iterate arrays.

2) Explore map(), forEach(), filter(), sort(), reduce()
let arr = [1, 2, 3, 4];

arr.forEach(x => console.log(x));
let mapped = arr.map(x => x * 2);
let filtered = arr.filter(x => x > 2);
let sorted = arr.sort((a, b) => b - a);
let sum = arr.reduce((a, b) => a + b);


These methods simplify array operations and improve readability.

3) Complete DOM Manipulation
<p id="demo">Hello</p>
<button onclick="changeText()">Click</button>

<script>
function changeText() {
  document.getElementById("demo").innerText = "Welcome";
}
</script>


DOM manipulation allows changing HTML content dynamically using JavaScript.

4) Event key, mouse, addEventListener properties
document.addEventListener("keydown", function(e) {
  console.log(e.key);
});

document.addEventListener("click", function(e) {
  console.log(e.target);
});
Keyboard and mouse events detect user interactions using addEventListener().

5) Explore npm and npx
npm install react
npm init -y
npx create-react-app myApp


npm installs and manages packages.
npx runs packages without global installation.
