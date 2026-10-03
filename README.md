Tourism Tour Management Website

A web application for managing and booking travel tours, developed using PHP Laravel.

The project allows users to browse available tours, view detailed tour information, create an account, log in, and make tour bookings.

Features

 User Authentication
- User registration
- Login using email or username
- Logout
- Password hashing using Laravel authentication utilities
- Session-based authentication

Tour Management
- Display available tours
- Tour pagination
- View tour details
- Display tour schedules
- Display destinations included in a tour
- Display tour guides
- Display customer reviews
- Calculate average tour rating

 Tour Booking
- Book a selected tour
- Select number of participants
- Select payment method
- Automatically calculate total booking price
- Store booking information in the database
- Default booking status: `CHO_XAC_NHAN`

 Customer Information
- Store registered user information
- Link user accounts with customer information

 Technologies

 Backend
- PHP 8.2+
- Laravel 12
- Laravel Eloquent ORM

 Frontend
- Blade Template Engine
- HTML
- CSS
- JavaScript
- Tailwind CSS
- Vite
- Axios

 Database
- MySQL

Development Tools
- phpMyAdmin
- Composer
- npm
- Git
- GitHub

 Main Models

The application includes several main entities:

- User
- Customer
- Tour
- Booking
- Tour Guide
- Schedule
- Destination
- Review


 Installation

 1. Clone the repository

git clone https://github.com/VThanh-Huy/Tour_Management_Website.git

Move into the project directory:
cd Tour_Management_Website

2. Install PHP dependencies
_composer install_
3. Install frontend dependencies
_npm install_

4. Create the environment file
Copy .env.example:
_cp .env.example .env_
On Windows Command Prompt:
_copy .env.example .env_

5. Generate the application key
_php artisan key:generate_

6. Configure MySQL
Create a MySQL database for the project.
Then update the following values in .env:
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=your_database_name
DB_USERNAME=root
DB_PASSWORD=your_password
Replace the values with your own MySQL configuration.

7. Run database migrations
_php artisan migrate_
If the project contains seed data:
_php artisan db:seed_
Or run migrations and seeders together:
_php artisan migrate --seed_
8. Start the Laravel server
_php artisan serve_
The application will normally be available at:
http://127.0.0.1:8000

9. Start Vite
Open another terminal and run:
_npm run dev_
Keep both Laravel and Vite running while developing the application.

**Development**
Useful Laravel commands:
```
php artisan route:list
```

Display all application routes.
```
php artisan migrate
```

Run database migrations.
```
php artisan migrate:fresh
```

Recreate the database tables.
```
php artisan migrate:fresh --seed
```

Recreate the database and insert seed data.
```
php artisan serve
```

Start the local Laravel development server.

Learning Outcomes

Through this internship project, I gained practical experience with:

- Developing a web application using PHP and Laravel
- Working with the MVC architecture
- Building database models and relationships using Eloquent ORM
- Connecting Laravel with MySQL
- Implementing user registration and authentication
- Working with sessions
- Implementing tour booking workflows
- Performing CRUD-related database operations
- Using Git and GitHub for basic version control
- Managing PHP dependencies with Composer
- Managing frontend dependencies using npm and Vite


Possible improvements for the project include:

- Admin dashboard
- Tour CRUD management for administrators
- Booking confirmation and cancellation
- User booking history
- Online payment integration
- Search and filtering for tours
- Role-based access control
- Improved validation and error handling
- Responsive UI improvements
- REST API development
- Automated testing

