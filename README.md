# Pro-Rated Refund Calculator

A simple, modern web-based calculator for computing pro-rated refunds based on service start and end dates.

![screenshot](screenshot.png)

---

## 🧮 Overview

This single-page HTML/JavaScript app helps calculate refunds proportionate to the unused portion of a product or service.

**Formula:**

```
refund = price × (remaining_days ÷ total_duration)
```

**Inputs:**

* **Reference Date** – The start of the service.
* **End of Service Date** – The date the service ends.
* **Price** – The total amount paid.
* **Duration (days)** – The full service period in days.

**Outputs:**

* Days used / remaining
* Percent used / remaining
* Pro-rated refund amount (rounded to two decimals)

---

## ⚙️ Features

✅ Clean responsive layout with dark mode aesthetics
✅ Real-time calculations
✅ Copy button for numeric-only refund values
✅ Smart date handling (timezone-safe UTC calculation)
✅ Query-string presets for all input fields
✅ Graceful fallbacks and validation for invalid input

---

## 🔗 Query String Parameters

You can pre-populate any of the inputs by adding parameters to the URL:

```
?price=99.95&duration=365&refDate=2025-01-01&endDate=2025-11-05
```

**Supported aliases:**

| Field          | Aliases                                |
| -------------- | -------------------------------------- |
| Reference Date | `refDate`, `ref`, `start`, `startDate` |
| End Date       | `endDate`, `end`, `stop`, `stopDate`   |
| Price          | `price`, `amount`, `total`             |
| Duration       | `duration`, `days`, `term`, `length`   |

If parameters are missing or invalid, default values are applied automatically.

---

## 🚀 Usage

1. Download or clone this repository.
2. Open `index.html` in any modern browser.
3. Optionally append query parameters to pre-fill fields.
4. Enter your data and view the instant calculation.
5. Click **Copy** to copy just the numeric refund amount.

---

## 💡 Example

Suppose a customer paid **$100** for a **365-day** subscription starting **Jan 1, 2025**, and canceled on **Jul 1, 2025**.

* Used days: 181
* Remaining days: 184
* Refund = 100 × (184 ÷ 365) ≈ **$50.41**

---

## 🧰 Tech Stack

* **HTML5** – Structure and layout
* **CSS3** – Minimal, modern, dark-themed design
* **Vanilla JavaScript** – Calculation logic, dynamic UI, clipboard handling

No dependencies, frameworks, or build tools required.

---

## 🧑‍💻 Contributing

Pull requests are welcome! To contribute:

1. Fork this repository.
2. Create a new branch: `git checkout -b feature/my-feature`.
3. Commit your changes: `git commit -m "Added feature X"`.
4. Push to your branch and open a pull request.

---

## 📄 License

This project is licensed under the **MIT License**.

---

© 2025 Andrew Douglas / Piper’s Dojo – All rights reserved.
