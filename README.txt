SafeRide - School Transport Management System (PHP 8 + MySQL/MariaDB + vanilla JS)

SETUP (XAMPP)
1. Install XAMPP (latest, PHP 8.x). Open XAMPP Control Panel and Start Apache and MySQL.
2. Copy the "saferide" folder into  C:\xampp\htdocs\
3. Open http://localhost/saferide/setup.php  -> creates the database "saferide", tables and demo data.
4. Delete setup.php, then open http://localhost/saferide/
5. Logins: admin/admin123, driver/driver123, parent/parent123
If your MySQL root has a password, edit DB_PASS in config.php and the PDO line in setup.php.

SECURITY CONTROLS: password_hash/verify, prepared statements (PDO), role-based access on every API action,
CSRF token, session ID regeneration, account lockout (3 fails -> 60 s), output escaping, security headers.
FILES: schema.sql (ER/table evidence), config.php, api.php (backend), index.php + assets/ (frontend).
