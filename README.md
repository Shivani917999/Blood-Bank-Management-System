# Blood-Bank-Management-System
# 
The Blood Bank Management System is a web-based application designed to facilitate the management of blood donation, storage, and distribution processes in blood banks and hospitals. It provides a centralized platform for donors, recipients, and blood bank staff to efficiently manage blood inventory, donation events, and requests.

## Features

- **User Management**: Registration, login, and profiles for donors, recipients, and staff.
- **Donor Management**: Record donor information, track donation history, and schedule appointments.
- **Blood Inventory**: Manage blood units by type, quantity, and expiry date.
- **Blood Requests**: Receive, process, and track requests from hospitals or recipients.
- **Donation Camps**: Schedule and manage blood donation events, track attendance.
- **Reports and Analytics**: Generate reports on inventory, donations, and distributions, with visualizations.
- **Admin Panel**: Manage system settings, users, permissions, and backups.
- **Security**: Secure authentication, role-based access control, data encryption.
- **Accessibility**: Ensure usability across devices and compliance with accessibility standards.
- **Feedback and Support**: Provide channels for feedback and assistance.

<h3>Technologies Used</h3>

<h4>Frontend:</h4>
<ul style="list-style-type: square;"> 
<li> JSP(JavaServerPage)</li>
<li>HTML</li>
<li>CSS for styling</li>
</ul>

<h4>Backend:</h4>
<ul style="list-style-type: square;"> 
<li>JDBC(DataBase Connectivity)</li>
<li>MYSQL</li>
<li>Servlets</li>

</ul>
# Blood Bank Management System

This project is a Blood Bank Management System developed using Apache Tomcat server.

## Getting Started

### 1. Clone the Repository

Clone the GitHub repository to your local machine using Git:

```bash
git clone https://github.com/yourusername/blood-bank-management-system.git
 ```
### 2. Install Apache Tomcat
 ```Download and install Apache Tomcat from the official website.```
### 3. Deploy the Project
Copy the project files into the Tomcat webapps directory.

### 4. Start Tomcat Server
Navigate to the Tomcat installation directory and run the startup script:

 ```./bin/startup.sh    # On Unix-like systems (Linux, macOS) ```
```.\bin\startup.bat   # On Windows```

### 5. Access the Application
Once Tomcat is running, open a web browser and navigate to ```http://localhost:8080/blood-bank-management-system.```

### 6. Configure Database
If your application uses a database, ensure that your database server is running. Update the database connection settings in your project configuration files to point to your local database server.

## Usage

1. **Donors**: Register, donate blood, manage profile.
2. **Recipients**: Request blood, track status.
3. **Administrators**: Manage users, inventory, donation camps.
4. **General Users**: Access system, navigate dashboard, submit requests, manage profile.

## Database Schema

### 1. Users Table

- **user_id**: A unique identifier for each user.
- **username**: The username used for logging into the system.
- **password**: The hashed password for user authentication.
- **role**: Specifies the role of the user (e.g., Donor, Recipient, Administrator).

### 2. Donors Table

- **donor_id**: A unique identifier for each donor.
- **user_id**: Foreign key linking to the Users table.
- **name**: The name of the donor.
- **blood_type**: The blood type of the donor.
- **phone**: The phone number of the donor.
- **email**: The email address of the donor.
- **last_donation_date**: The date of the donor's last blood donation.

### 3. Recipients Table

- **recipient_id**: A unique identifier for each recipient.
- **user_id**: Foreign key linking to the Users table.
- **name**: The name of the recipient.
- **blood_type**: The blood type required by the recipient.
- **hospital**: The hospital where the recipient is located.
- **phone**: The phone number of the recipient.
- **email**: The email address of the recipient.
- **request_status**: Indicates the status of the recipient's blood request (e.g., Pending, Fulfilled).

### 4. Blood Inventory Table

- **blood_id**: A unique identifier for each blood unit.
- **blood_type**: The blood type of the unit.
- **quantity**: The quantity of blood units available.
- **expiry_date**: The expiry date of the blood unit.

### 5. Donation Requests Table

- **request_id**: A unique identifier for each donation request.
- **recipient_id**: Foreign key linking to the Recipients table.
- **blood_type**: The blood type requested by the recipient.
- **quantity**: The quantity of blood units requested.
- **request_date**: The date when the request was made.
- **status**: Indicates the status of the request (e.g., Pending, Approved, Rejected).

<h3>Contributing</h3>
<p> Contributions to this project are welcome! If you would like to contribute, please follow these steps:</p>
<ol>
<li>Fork the repository.</li>
<li>Create a new branch for your feature or bug fix.</li>
<li>Make your changes and test thoroughly.</li>
<li>Create a pull request with a detailed description of your changes.</li>
<ol>



