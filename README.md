# **Applying Filters to SQL Queries**

## **Project Description**  
In this project, I analyzed security-related data to identify potential risks in login attempts and employee machine updates within a large organization. Using **SQL**, I retrieved and filtered data from the `log_in_attempts` and `employees` tables to detect suspicious activity and ensure compliance with security policies.  

The focus was on applying **SQL filtering techniques**, including `AND`, `OR`, `NOT`, and `LIKE`, to extract meaningful insights efficiently.  

---

## **Key Queries & Analysis**  

### **1. Retrieve After-Hours Failed Login Attempts**  
**Objective**: Identify failed login attempts that occurred outside business hours.  
**Query Highlights**:  
- Filtered login attempts occurring **after 18:00**.  
- Used `WHERE` with conditions on `login_time` and `success = FALSE`.  

### **2. Retrieve Login Attempts on Specific Dates**  
**Objective**: Extract login records for **2022-05-08 and 2022-05-09**.  
**Query Highlights**:  
- Used `WHERE` with an `OR` operator for **date filtering**.  

### **3. Retrieve Login Attempts Outside Mexico**  
**Objective**: Detect login attempts from locations **excluding Mexico**.  
**Query Highlights**:  
- Applied `NOT LIKE 'MEX%'` to filter out records labeled as **MEX** or **MEXICO**.  

### **4. Retrieve Employees in the Marketing Department (East Building)**  
**Objective**: Identify employees in **Marketing** located in the **East building**.  
**Query Highlights**:  
- Used `WHERE` with `AND` to filter department and office location.  
- Applied `LIKE 'East%'` to match building codes dynamically.  

### **5. Retrieve Employees in Finance or Sales**  
**Objective**: List employees working in **Finance or Sales**.  
**Query Highlights**:  
- Used `WHERE` with `OR` to include both departments.  

### **6. Retrieve Employees Not in IT**  
**Objective**: Extract a list of employees **excluding the IT department**.  
**Query Highlights**:  
- Used `WHERE` with `NOT` to exclude **Information Technology** staff.  

---

## **Summary**  
In this project, I leveraged **SQL filtering techniques** to extract key insights from organizational data, focusing on security monitoring and employee access tracking. The queries demonstrated proficiency in:  
- **Logical filtering** using `AND`, `OR`, and `NOT`.  
- **Pattern matching** with `LIKE` and wildcard `%`.  
- **Security-focused data analysis** using structured queries.  

---

## **Usage & Execution**  
To run these queries, connect to a **MariaDB or MySQL database**, ensure you have access to the `log_in_attempts` and `employees` tables, and execute the queries in a SQL environment.  
