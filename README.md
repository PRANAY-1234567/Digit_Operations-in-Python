📊 Digit Operations in Python

This repository contains simple Python programs to perform basic operations on digits of a number.

1️⃣ Print Digits of a Number (Reverse Order)

📌 Description

This program extracts and prints each digit of a number one by one starting from the last digit.

💻 Code
num = 5873

while num > 0:
    last_digit = num % 10
    print(last_digit)
    num = num // 10

	
▶️ Output
3
7
8
5

<img width="589" height="749" alt="Screenshot 2026-06-09 220203" src="https://github.com/user-attachments/assets/0f860c9c-19a1-4ecb-9147-1ee5004c09c3" />

🧠 How It Works

% 10 gives the last digit.
// 10 removes the last digit.
Loop continues until the number becomes 0.
⏱️ Time Complexity
O(d)

where d = number of digits.

💾 Space Complexity
O(1)


2️⃣ Count Digits Using Loop
📌 Description

This program counts the number of digits in a given integer using a loop.

💻 Code
n = 5438
count = 0

while n > 0:
    count += 1
    n = n // 10

print(count)
▶️ Output
4
🧠 How It Works

For each iteration:

One digit is removed using // 10.
Counter increases by 1.
When the number becomes 0, the counter stores the total digits.
⏱️ Time Complexity
O(d)
💾 Space Complexity
O(1)
3️⃣ Count Digits Using log10()
📌 Description

This program finds the number of digits using a mathematical formula instead of a loop.

💻 Code
from math import log10

n = 5438
digits = int(log10(n)) + 1

print(digits)
▶️ Output
4
🧠 Formula Used

Digits=⌊log
10
	​

(n)⌋+1

Example:

log10(5438) ≈ 3.735
int(3.735) + 1 = 4
⏱️ Time Complexity
O(1)
💾 Space Complexity
O(1)
🚀 Concepts Covered
Modulus Operator (%)
Floor Division (//)
While Loop
Digit Extraction
Digit Counting
Mathematical Functions (log10)
Time Complexity
Space Complexity
👨‍💻 Author

Pranay Jadhao

Electronics & Telecommunication Engineer
Aspiring Software & Embedded Systems Engineer
