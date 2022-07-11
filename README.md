# LaraGigs

An app for listing Laravel gigs/jobs. This project is based on Traversy Media's YouTube "[Laravel From Scratch 2022](https://www.youtube.com/watch?v=MYyJ4PuL4pY)" course.

![image](https://user-images.githubusercontent.com/66157842/178218275-90480411-c779-4d94-b379-9806b9377563.png)

## Usage

### Database Setup
This app uses MySQL. To use something different, open up config/Database.php and change the default driver.

To use MySQL, make sure you install it, setup a database and then add your db credentials(database, username and password) to the .env.example file and rename it to .env

### Migrations
To create all the nessesary tables and columns, run the following
```
php artisan migrate
```

### Seeding The Database
To add the dummy listings with a single user, run the following
```
php artisan db:seed
```

### File Uploading
When uploading listing files, they go to "storage/app/public". Create a symlink with the following command to make them publicly accessible.
```
php artisan storage:link
```

### Running Then App
Upload the files to your document root, Valet folder or run 
```
php artisan serve
```

## License

The LaraGigs app is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
