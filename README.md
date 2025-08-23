 Employee Data Management (AWS Project)

 Project Overview
This is a simple AWS-based web application that allows you to store and retrieve employee details.  
It demonstrates the use of **Serverless Architecture** using AWS services: API Gateway, Lambda, and DynamoDB.

---

 Architecture
1. Frontend → HTML, CSS, JavaScript (AJAX calls with jQuery)  
2. API Gateway → Acts as the entry point for API requests  
3. AWS Lambda → Two Python functions:
   - `insertEmployeeData.py` → Save employee details into DynamoDB
   - `getEmployees.py` → Fetch all employees from DynamoDB
4. DynamoDB → NoSQL database that stores employee records

---


 Project Structure
Employee-Data-AWS-Project/
│── index.html             Frontend UI
│── scripts.js             JavaScript (AJAX calls to API Gateway)
│── insertEmployeeData.py  Lambda function to insert data
│── getEmployees.py        Lambda function to fetch data
└── README.md              Project documentation



---

 Features
- Add Employee Data (Employee ID, Name, Department, Salary)  
- View All Employees stored in DynamoDB  
- Serverless Implementation using AWS Lambda + API Gateway  
- NoSQL Database(DynamoDB)  

---

 How It Works
1. User enters employee details in the web form (index.html)  
2. `scripts.js` makes an AJAX POST request to API Gateway  
3. API Gateway triggers Lambda function (insertEmployeeData.py) → saves data into DynamoDB  
4. When user clicks View All Employees, another request is sent to API Gateway  
5. API Gateway triggers Lambda function (getEmployees.py) → retrieves all data from DynamoDB  
6. Data is displayed dynamically in the HTML table  

---

Demo Screenshot
(Add a screenshot of your webpage here after hosting on AWS or running locally)

---

 Tech Stack
- Frontend: HTML, CSS, JavaScript (jQuery)  
- Backend: AWS Lambda (Python)  
- Database: AWS DynamoDB  
- API Management: AWS API Gateway  

---

 Steps to Deploy on AWS
1. Create a DynamoDB table named `employeeData` with `employeeid` as the primary key.  
2. Create two AWS Lambda functions:
   - Upload `insertEmployeeData.py` → for inserting data  
   - Upload `getEmployees.py` → for fetching data  
3. Create an API Gateway and link it with both Lambda functions (`POST` for insert, `GET` for fetch).  
4. Copy your API Gateway endpoint into `scripts.js` (replace the `API_ENDPOINT` value).  
5. Open `index.html` in your browser → Test the application.  

---

 Author
  Ankush Tupone  
  Aspiring Cloud & DevOps Engineer | AWS & Linux Enthusiast  

---

License
This project is for educational/demo purposes as part of AWS learning.
