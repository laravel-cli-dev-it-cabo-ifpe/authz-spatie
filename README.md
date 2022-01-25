# authz-spatie

# Install and setup the dependencies

npm install 
npm run dev

# Creating Controller
php artisan make:controller UserController --resource

php artisan make:controller RoleController --resource

php artisan make:controller PermissionController --resource

php artisan make:controller PostController --resource

# Creating Table Seeder
php artisan make:seeder PermissionTableSeeder

php artisan make:seeder RoleTableSeeder

php artisan make:seeder UserTableSeeder

# Feed Table Seeder
php artisan db:seed --class=RoleTableSeeder

php artisan db:seed --class=UserTableSeeder

php artisan db:seed --class=PermissionTableSeeder

# Migrage changes
php artisan migrate
