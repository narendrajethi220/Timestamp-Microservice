> A simple Node.js and Express microservice that returns Unix and UTC timestamps based on a user-supplied date or the current time. Built as part of FreeCodeCamp’s Backend Development and APIs certification.

![Screenshot (67)](https://github.com/user-attachments/assets/df45185e-b136-4cdc-95ae-d5df18113287)
![Screenshot (68)](https://github.com/user-attachments/assets/29e7ef0f-8c69-461a-94f5-2dbf4ff5d0e4)

---

### 📄 `README.md`

````markdown
# Timestamp Microservice

This is a simple full-stack JavaScript application built using **Node.js** and **Express**. It is part of the [FreeCodeCamp Backend Development and APIs Certification](https://www.freecodecamp.org/learn/back-end-development-and-apis/) and fulfills the requirements for the **Timestamp Microservice** project.

## 📋 Project Objective

Build an API endpoint `/api/:date?` that accepts a date string or timestamp and returns a JSON response with the date in both **Unix timestamp** and **UTC string** format.

## 🛠️ Technologies Used

- Node.js
- Express.js

## 🚀 How It Works

### Route: `/api/:date?`

- If `:date` is **empty**, return the current time in both Unix and UTC formats.
- If `:date` is a valid **date string** or **Unix timestamp**, return both formats.
- If `:date` is invalid, return:
  ```json
  { "error": "Invalid Date" }
````

### Example Responses

```json
GET /api/1451001600000
{
  "unix": 1451001600000,
  "utc": "Fri, 25 Dec 2015 00:00:00 GMT"
}
```

```json
GET /api/invalid-date
{
  "error": "Invalid Date"
}
```

## ✅ User Stories & Requirements

* [x] API endpoint `/api/:date?` handles empty, valid, and invalid dates.
* [x] Returns:

  * `unix` timestamp in milliseconds
  * `utc` date string in RFC1123 format
* [x] Passes all FreeCodeCamp automated test cases

## 📦 Installation and Running Locally

1. Clone the repository:

   ```bash
   git clone https://github.com/narendrajethi220/Timestamp-Microservice.git
   cd Timestamp-Microservice
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Start the development server:

   ```bash
   npm start
   ```

4. Visit:

   ```
   http://localhost:3000/api
   ```

---

### 🎓 Certification
This project is part of the **FreeCodeCamp Backend Development and APIs** certification.
