Laravel User Management System
This is a simple Laravel web application that lets users register, log in, and log out. It uses role-based authentication with two roles: Admin and User. Admins can manage users by creating, updating, and deleting them from a dashboard.

Features
User registration

Login and logout

Role-based access control (Admin and User)

Admin dashboard for user management:

View all users

Create new users

Edit existing users

Delete users

Technologies Used
Laravel (PHP framework)

Blade (Laravel's template engine)

MySQL (database)

Laravel Breeze (for authentication setup)

Bootstrap (for styling)

Project Structure
pgsql
Copy
Edit
app/
├── Http/
│   ├── Controllers/
│   │   └── Admin/
│   │       └── UserController.php  (User management by admin)
│   └── Middleware/
│       └── AdminMiddleware.php     (Restricts routes to admin only)
resources/
└── views/
    ├── admin/
    │   └── users/
    │       ├── index.blade.php     (List users)
    │       ├── create.blade.php    (Add user)
    │       └── edit.blade.php      (Edit user)
How to Run the Project
Clone the repository:

bash
Copy
Edit
git clone https://github.com/your-username/laravel-user-management.git
cd laravel-user-management
Install PHP dependencies:

nginx
Copy
Edit
composer install
Set up environment file and generate app key:

bash
Copy
Edit
cp .env.example .env
php artisan key:generate
Open the .env file and update your database credentials:

ini
Copy
Edit
DB_DATABASE=your_database_name
DB_USERNAME=your_database_user
DB_PASSWORD=your_database_password
Install frontend dependencies and build assets (optional):

arduino
Copy
Edit
npm install
npm run dev
Run database migrations and seed the admin user:

css
Copy
Edit
php artisan migrate --seed
Start the Laravel development server:

nginx
Copy
Edit
php artisan serve
Open your browser and visit:

cpp
Copy
Edit
http://127.0.0.1:8000
Admin User Credentials
Email: admin@example.com

Password: password
