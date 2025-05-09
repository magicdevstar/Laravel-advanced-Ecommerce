
## Getting Started Step by Step
1. In your root folder, clone the project file using git clone
2. Open terminal (bash/cmd). Then go to project folder using command

3. Then install required files and libraries using 

```sh
composer install
```

4. Then create a .env file and generate key for this project using command 

```sh
cp .env.example .env

php artisan key:generate
```

5. Then compile all CSS & JS files together using this command

```sh
npm install && npm run dev
```

or

```sh
yarn install && yarn run dev
```
6. Create a database in MYSQL and connect it with your project via updating .env file.
7. After connecting the db with project, then run command 

```sh
php artisan migrate:fresh --seed
```

After completing the migration and seeding of db, you will have 2 user ready for login in this project. 
A.  Admin -> Admin
    Email -> admin@gmail.com
    Pass -> 12345678

B.  User -> User
    Email -> user@gmail.com
    Pass -> 12345678

Finally we are ready to run our project using this command 

```sh
php artisan serve
```
