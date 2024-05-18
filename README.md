# E-BMS
- The Blood Management System is a comprehensive web-based application developed using MySQL, PHP, HTML, CSS, and JavaScript. This project aims to streamline and enhance the management of blood donations and transfusions, making the process more efficient and accessible for both donors and healthcare providers.

## Key Features:

### Donor Registration and Management:
- A user-friendly interface for donors to register and update their profiles.
- Secure storage of donor information in a MySQL database.
- Automated notifications for blood donation reminders and eligibility status.

### Blood Donation and Request Handling:
- **Donor Functionality:** Donors can easily schedule and record blood donations.
- Patient Functionality: Patients or their representatives can request specific blood types through the system.
- Seamless processing of blood requests from hospitals and clinics.
- Prioritization and matching of blood requests based on urgency and compatibility.
- Comprehensive log of all donations and requests for transparency and accountability.

### Blood Inventory Management:
- Real-time tracking of blood stock levels across different blood types and components.
- Easy-to-use dashboard for managing blood inventory and expiry dates.
- Alerts for low stock levels and upcoming expiration of blood units.

### Request Handling:
- Seamless processing of blood requests from hospitals and clinics.
- Prioritization and matching of blood requests based on urgency and compatibility.
- Comprehensive log of all transactions for transparency and accountability.

### Reporting and Analytics:
- Detailed reports on donor activity, blood usage, and inventory status.
- Data visualization tools for better understanding of trends and patterns.
- Exportable reports for administrative and regulatory purposes.

## Technologies Used:
- HTML & CSS: Front-end technologies for creating a responsive and user-friendly interface.
- JavaScript: Enhances interactivity and user experience with dynamic content updates.
- MySQL: Database management system for storing and retrieving data efficiently.
- PHP: Server-side scripting language for handling the application logic.

## Installation and Execution Steps
### Clone the Repository
First, clone the repository to your local machine using the following command:
```sh
git clone https://github.com/Utsav-7/E-BMS.git
```
### Set Up the Database
- Start your XAMPP or WAMP server.
- Open phpMyAdmin in your web browser (usually http://localhost/phpmyadmin).
- Create a new database named blood_management.
- Import the SQL file located in the database folder of the cloned repository:
  - Click on the Import tab.
  - Choose the file blood_management.sql from the database folder.
  - Click Go to import the database.

### Configure the Project
1. Navigate to the project directory:
``` 
cd blood-management-system
```
2. Open the **'config.php'** file located in the root directory.
3. Update the database configuration details:
```
<?php
    // Enter your host name, database username, password, and database name.
    // If you have not set database password on localhost then set empty.
     $con = mysqli_connect("localhost","root","","user");
    // Check connection
    if (mysqli_connect_errno()){
        echo "Failed to connect to MySQL: " . mysqli_connect_error();
    }
?>
```
### Start the Server
- Move the project directory to the htdocs folder of your XAMPP installation (usually C:\xampp\htdocs).
- Open your web browser and go to http://localhost/blood-management-system.
### Access the Application
- **Donor Interface:** To register and donate blood.
- **Patient Interface:** To request blood.
- **Admin Interface:** For managing donors, requests, and inventory.

<br>

- This Blood Management System not only optimizes the workflow of blood donation and transfusion but also ensures the safety and reliability of the blood supply chain, ultimately contributing to better healthcare outcomes. Donors can effortlessly give blood, and patients can conveniently request blood, making the system highly effective and user-centric.
