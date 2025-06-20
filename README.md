# Jagdish Transport Management System

Jagdish Transport Management System is a web-based application designed to automate and manage the day-to-day operations of a transport company. The system provides tools for managing vehicles, tracking trips, handling billing and invoicing, and maintaining customer information.

## Author

<a href="https://github.com/Atharva-2510/Jagdish-Transport/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=Atharva-2510/Jagdish-Transport" />
</a>

## Features

### Vehicle Management
- Register and track vehicles
- Categorize vehicles by type
- Manage vehicle maintenance schedules
- Generate vehicle statements

### Trip Management
- Create and track trip vouchers
- Manage trip areas and routes
- Record trip details and expenses

### Billing & Invoicing
- Generate party bills and invoices
- Configure bill settings
- Track payment status
- Manage different rate types (Freight, CDWT, Waiting, etc.)

### Customer Management
- Maintain party (customer) master records
- Track customer transactions
- Manage customer locations and areas

### User Management
- Secure user authentication and authorization
- User profile management
- Role-based access control

### Dashboard & Reporting
- View key performance indicators
- Access recent transactions
- Generate various reports

## Technology Stack

### Backend
- Java 17
- Spring Boot 3.4.3
- Spring Security
- Spring Data JPA
- Hibernate
- MySQL Database

### Frontend
- Thymeleaf templating engine
- HTML/CSS/JavaScript
- Bootstrap (assumed)

### Additional Tools
- Maven for dependency management
- Spring Mail for email notifications
- Lombok for reducing boilerplate code
- Hibernate Validator for data validation

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Atharva-2510/Jagdish-Transport.git
   cd Jagdish-Transport
   ```

2. **Configure the database**
   - Create a MySQL database named `jagdishtransport_db`
   - Update the database credentials in `src/main/resources/application.properties`
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/jagdishtransport_db?createDatabaseIfNotExist=true
   spring.datasource.username=your_mysql_username
   spring.datasource.password=your_mysql_password
   ```

3. **Configure email settings (for notifications)**
   - Update the email configuration in `src/main/resources/application.properties`
   ```properties
   spring.mail.username=your_email@gmail.com
   spring.mail.password=your_app_password
   ```

4. **Build the application**
   ```bash
   mvn clean install
   ```

5. **Run the application**
   ```bash
   mvn spring-boot:run
   ```
   
   The application will be available at `http://localhost:8081`

## Project Structure

```
src/main/java/com/example/JagdishTransport/
├── Config/                  # Configuration classes
├── Controller/              # Web controllers
├── dto/                     # Data Transfer Objects
├── model/                   # Entity classes
├── repository/              # Data access interfaces
├── service/                 # Business logic
│   └── impl/                # Service implementations
└── JagdishTransportApplication.java  # Main application class
```

## Security

The application implements Spring Security with:
- Form-based authentication
- BCrypt password encoding
- Role-based access control
- CSRF protection (disabled for specific endpoints)

## Database

The application uses MySQL with JPA/Hibernate for data persistence. The database schema is automatically created and updated using Hibernate's `ddl-auto=update` feature.

## Screenshots

### Login Page
![Login Page](img/Login.png)
*User login page*

### Dashboard
![Dashboard](img/Dashboard.png)
*Main dashboard showing key metrics and recent activities*

### Vehicle Statement
![Vehicle Management](img/vehicalStatement.png)
*Vehicle registration and management interface*

### Trip Voucher
![Trip Voucher](img/TripVoucher.png)
*Trip voucher creation and tracking*

### Trip Voucher table
![Trip Voucher](img/TripVoucherTable.png)
*Trip voucher creation and tracking*

### Party Bill
![Party Bill](img/PartyBill.png)
*Party bill generation and management*

### Party statement
![Party Bill](img/PartyStatement.png)
*Party bill generation and management*

### Vehicle Statement
![Vehicle Master](img/vehicalStatement.png)
*Vehicle registration and management interface*


## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the [MIT License](LICENSE) - see the LICENSE file for details.

## Contact

Name: atharvapimparkar1416@gmail.com  

Project Link: https://github.com/Atharva-2510/Jagdish-Transport

