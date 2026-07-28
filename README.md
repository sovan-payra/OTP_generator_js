# 🔐 Random OTP Generator

A simple **6-digit OTP (One-Time Password) Generator** built using JavaScript. This project generates a random number between `100000` and `999999` every time the program runs.

## 🚀 Features

* Generates a random **6-digit OTP**
* Simple and lightweight
* Uses built-in JavaScript methods
* No external libraries or dependencies
* Beginner-friendly JavaScript project

## 🛠️ Technologies Used

* **JavaScript**

## 📂 Project Structure

```text
otp-generator/
│
├── script.js
└── README.md
```

## 💻 Code

```javascript
function generateOTP() {
    // Generate a random number between 100000 and 999999
    const otp = Math.floor(100000 + Math.random() * 900000);
    return otp;
}

console.log(generateOTP());
```

## ⚙️ How It Works

The OTP is generated using:

```javascript
Math.floor(100000 + Math.random() * 900000)
```

Here's what happens:

1. `Math.random()` generates a random decimal number from `0` up to, but not including, `1`.
2. Multiplying it by `900000` creates a value from `0` up to just under `900000`.
3. Adding `100000` ensures the generated number is always six digits.
4. `Math.floor()` removes the decimal part.

Example output:

```text
583291
```

Each time the program runs, a different OTP can be generated.

## ▶️ How to Run

Make sure **Node.js** is installed on your computer.

Open a terminal inside the project directory and run:

```bash
node script.js
```

The generated OTP will appear in the terminal.

Example:

```text
$ node script.js
748215
```

## 📌 Use Cases

This project can be used as a starting point for:

* OTP verification systems
* Login verification demos
* Registration verification demos
* Password reset flows
* Learning JavaScript random number generation

## 🔒 Security Note

This project uses `Math.random()`, which is suitable for learning and simple demonstrations but **should not be used to generate security-sensitive OTPs in production**.

For real authentication systems, use a cryptographically secure random number generator such as the Web Crypto API or Node.js `crypto` module.

## 🔮 Future Improvements

* Add an OTP expiration timer
* Add OTP verification
* Generate OTPs using cryptographically secure randomness
* Send OTPs through email or SMS
* Build a user interface with HTML and CSS
* Add resend OTP functionality

## 📄 License

This project is open source and available for educational and personal use.

---

⭐ If you found this project helpful, consider giving the repository a star!
