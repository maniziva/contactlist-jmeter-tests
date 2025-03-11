# **Contact List App - API Testing with JMeter**  

This repository contains JMeter test scripts for performance and API testing of the **Contact List App** ([Live Site](https://thinking-tester-contact-list.herokuapp.com/)). It includes test plans for **functional validation, load testing, and performance benchmarking** to ensure the application's backend services are reliable and scalable.  

---

## **📌 Features**  
✔️ JMeter test scripts for **REST API validation**  
✔️ **Authentication token extraction** for secure requests  
✔️ Load & performance testing scenarios  
✔️ **Assertions** for response code and response time  
✔️ Automated test execution setup  
✔️ **Detailed reports and logs**  

---

## **🛠️ Setup Instructions**  

### **1️⃣ Prerequisites**  
- **Install JMeter**: [Download Here](https://jmeter.apache.org/download_jmeter.cgi)  
- **Install JSON Extractor Plugin** (Optional, for better response handling)  

---

### **2️⃣ How to Run Tests**  

#### **👉 1. Open JMeter**  
- Launch **Apache JMeter** and open the provided `.jmx` test plan.  

#### **👉 2. Set Environment Variables** (Optional)  
- Modify the **Base URL** in the **User Defined Variables** section:  BASE_URL = https://thinking-tester-contact-list.herokuapp.com/
#### **👉 3. Run API Tests**  
- Click **Run ▶️** to execute test cases.  

---

## **🚀 API Test Scenarios**  

### **✅ 1. Login API Test**  
- **Request**: `POST /users/login`  
- **Extracts authentication token using JSON Extractor.**  
- **Response Assertion**: Checks if response code is `200`.  

### **✅ 2. Logout API Test**  
- **Request**: `POST /users/logout`  
- **Uses extracted authentication token in "Authorization" header.**  
- **Response Assertion**: Ensures response code is `200`.  

### **✅ 3. Contact List CRUD Operations**  
- **GET /contacts** → Fetches contact list  
- **POST /contacts** → Adds a new contact  
- **PUT /contacts/{id}** → Updates a contact  
- **DELETE /contacts/{id}** → Deletes a contact  
- **Assertions**: Ensures correct response codes & data validation  

### **✅ 4. User List CRUD Operations**  
- **GET /users/me** → Fetches user data  
- **PATCH /users/me** → Updates a user data  
- **Assertions**: Ensures correct response codes & data validation  

---

## **🔍 Assertions Used**  
- **Response Code = 200** (Successful API Call)  
- **Response Time < 2000ms** (Performance Benchmark)  
- **JSON Path Validation** (Ensures correct API response structure)  

---

## **📊 Reports & Logs**  
- View **JMeter Summary Report** for performance analysis.  
- Use **Listeners** like **View Results Tree** for debugging API responses.  

---

## **📌 Notes**  
⚡ Ensure you use **correct credentials** for login API.  
⚡ If authentication fails, check **token extraction settings**.  
⚡ Update **thread count** for **load testing** scenarios.  

---

### **👨‍💻 Contributors**  
- **Manikandan Adaikalam**  

### **📩 Contact - https://maniziva.github.io/MyPortfolio/**  
If you have any issues or suggestions, feel free to open an **issue**! 🚀  
