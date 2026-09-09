# Student API Test Suite

REST API testing suite built with Postman and a local `json-server` mock backend.

---

## Tech Stack
* **Mock Server:** `json-server`
* **Runtime:** Node.js
* **API Testing Tool:** Postman
* **Database:** `students.json` (Local JSON database)

---

## Endpoints Tested

* `GET /students` — Retrieve all students (`200 OK`)
* `POST /students` — Create student record (`201 Created`)
* `GET /students/:id` — Fetch record using ID (`200 OK`)
* `PUT /students/:id` — Update existing student details (`200 OK`)
* `DELETE /students/:id` — Remove student record (`200 OK`)
* `GET /students/:id` — Verify record deletion (`404 Not Found`)

---

## Setup & Execution

### 1. Install Dependencies
```bash
npm install
```

### 2. Start Mock Server
```bash
npm start
```
The mock API will run at `http://localhost:3000/students`. Keep this terminal window open.

### 3. Run Tests in Postman
1. Open Postman and click **Import**.
2. Select the exported `.json` collection from this repository.
3. Open the collection runner and execute the requests sequentially.
