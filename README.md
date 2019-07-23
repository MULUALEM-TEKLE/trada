# trada

![trade logo](/trada.jpg)

## SetUp instructions 
### 1 | System Requirments
  __composer and npm must be installed__
  ```
  {
    sudo apt install composer;
    sudo apt install npm;
  }
  ```
  
  php 7.3.* must be used
  
  ### 2 | Cloning the repo 
  __clone this the repo to your local machine__
  
  ```
    git clone 
  ```

### 3 | Running the project
__fire up your server stack(xampp , lampp , wampp , mamp)__

*make sure you hav atleast Apache and MySql are running , the database and username specified in your .env file must exist in your data base. please verify via phpMyAdmin*

__migrate the databases__

*cd into the repo directory and run the following command*
```
php artisan migrate:fresh --seed
```
__start the server__

```
php artisan serve
```

__verify that its working via your browser__
