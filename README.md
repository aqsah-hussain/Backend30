# **Employee Management System API**

This is a RESTful API for managing employee records, including creating, reading, updating, and deleting employees. The project uses **Node.js**, **Express**, and **MongoDB**.

---

## **Features**
- **Create** a new employee record.
- **Fetch** all employee records.
- **Fetch** a single employee by ID.
- **Update** an existing employee record.
- **Delete** an employee record.

---

## **Technologies Used**
- **Node.js**: Backend runtime.
- **Express**: Web framework.
- **MongoDB**: NoSQL database.
- **Mongoose**: ODM for MongoDB.

---

## **Setup Instructions**

1. **Clone the repository**:
   ```bash
   git clone <repository_url>
2. **Navigate to the project directory**:
   - After cloning, go into the project folder by running:
     ```bash
     cd <project_directory>
     ```

3. **Install dependencies**:
   - Make sure you have **Node.js** installed. If not, [download it here](https://nodejs.org/).
   - Install the project dependencies using:
     ```bash
     npm install
     ```

4. **Create a `.env` file**:
   - In the root directory of the project, create a new file named `.env`.
   - Add the following content to `.env`:
     ```bash
     MONGO_URL="mongodb://localhost:27017/EmployeeTest"
     PORT=7788
     ```

5. **Start the server**:
   - Once all dependencies are installed and the `.env` file is set up, start the server by running:
     ```bash
     node server.js
     ```

6. **Test API endpoints**:
   - Open Postman or any API testing tool.
   - Use the **base URL** `http://localhost:7788/employee` to test the following API endpoints:
     - **POST** `/createEmployee`: To create a new employee.
     - **GET** `/getEmployees`: To fetch all employees.
     - **GET** `/getEmployee/:id`: To fetch a single employee by ID.
     - **PUT** `/updateEmployee/:id`: To update an employee by ID.
     - **DELETE** `/deleteEmployee/:id`: To delete an employee by ID.

---
## **API Endpoints**

| Method  | Endpoint                   | Description               |
|---------|----------------------------|---------------------------|
| **POST**| `/createEmployee`          | Create a new employee.    |
| **GET** | `/getEmployees`            | Fetch all employees.      |
| **GET** | `/getEmployee/:id`         | Fetch an employee by ID.  |
| **PUT** | `/updateEmployee/:id`      | Update an employee by ID. |
| **DELETE** | `/deleteEmployee/:id`    | Delete an employee by ID. |

---
##**Folder Structure**
project-directory/
│
├── controller/
│   └── EmployeeController.js  # API logic
│
├── models/
│   └── Employee.js            # MongoDB schema
│
├── routes/
│   └── EmployeeRoutes.js      # API routes
│
├── server.js                  # Entry point
├── .env                       # Environment variables
└── package.json               # Dependencies
---

## **Author**

- **Aqsah Hussain**

---