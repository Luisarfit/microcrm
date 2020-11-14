Voyager CRM Stable: v1.1

Login

Admin

URL: /admin/login

User: admin@admin.com Password: password.

SET UP

Requirements (Already covered with Docker deployment)

Apache/2.4.27 or greater. MySQL 5.7 or greater. PHP/7.2.24 or greater.

App Configuration

Add host voyager-crm.localhost, see Edit hosts. Create .env file from example.env and set it. Set db instead localhost in .env while using Docker.

Import database from database/updates/*update.sql into voyager1 DB with root user, at localhost host, 33063 port. Set APP_KEY=base64:wS4QdM09HXTVCzIpkp90ML1OkZZOjRKbf0IQZ6f0Cwk= at .env. Run composer install. Run php artisan storage:link. Run php artisan migrate.

Create Admin User Create Admin User: php artisan create-admin-user --user={email-here} Example: php artisan create-admin-user --user=admin@adlnetworks.com

Browse at voyager-crm.localhost.

Voyager Back Office at voyager-crm.localhost/admin.

CONTRIBUTION: Guidelines & Documentation

Database Key Fields, tables and or values:

users.email: Users email.

Git : Gitflow.

Back End: Laravel 7.x, Laravel Voyager.

Front End: Admin LTE, Bootstrap 4, Laravel Admin LTE, Font Awesome.

2020 Lum labs
