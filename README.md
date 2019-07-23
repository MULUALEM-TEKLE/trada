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
  __run the following on your terminal__
  
  ```
  composer global require laravel/installer
  ```
  _This error might arise_
  
  ```
  Your requirements could not be resolved to an installable set of packages.

  Problem 1
    - Installation request for laravel/installer ^2.1 -> satisfiable by laravel/installer[v2.1.0].
    - laravel/installer v2.1.0 requires ext-zip * -> the requested PHP extension zip is missing from your system.

  To enable extensions, verify that they are enabled in your .ini files:
    - /etc/php/7.3/cli/php.ini
    - /etc/php/7.3/cli/conf.d/10-mysqlnd.ini
    - /etc/php/7.3/cli/conf.d/10-opcache.ini
    - /etc/php/7.3/cli/conf.d/10-pdo.ini
    - /etc/php/7.3/cli/conf.d/20-calendar.ini
    - /etc/php/7.3/cli/conf.d/20-ctype.ini
    - /etc/php/7.3/cli/conf.d/20-exif.ini
    - /etc/php/7.3/cli/conf.d/20-fileinfo.ini
    - /etc/php/7.3/cli/conf.d/20-ftp.ini
    - /etc/php/7.3/cli/conf.d/20-gettext.ini
    - /etc/php/7.3/cli/conf.d/20-iconv.ini
    - /etc/php/7.3/cli/conf.d/20-json.ini
    - /etc/php/7.3/cli/conf.d/20-mbstring.ini
    - /etc/php/7.3/cli/conf.d/20-mysqli.ini
    - /etc/php/7.3/cli/conf.d/20-pdo_mysql.ini
    - /etc/php/7.3/cli/conf.d/20-phar.ini
    - /etc/php/7.3/cli/conf.d/20-posix.ini
    - /etc/php/7.3/cli/conf.d/20-readline.ini
    - /etc/php/7.3/cli/conf.d/20-shmop.ini
    - /etc/php/7.3/cli/conf.d/20-sockets.ini
    - /etc/php/7.3/cli/conf.d/20-sysvmsg.ini
    - /etc/php/7.3/cli/conf.d/20-sysvsem.ini
    - /etc/php/7.3/cli/conf.d/20-sysvshm.ini
    - /etc/php/7.3/cli/conf.d/20-tokenizer.ini
  You can also run `php --ini` inside terminal to see which files are used by PHP in CLI mode.

Installation failed, deleting ./composer.json.
  ```
  
  _in that case run the following commamd before and rerun the previous command_
  
  ```
  sudo apt-get install php7.3-zip
  ```
  __NOTE :__  _during this proccess some packages might not be installed correctly so try it again untill it succeeds_
  php 7.3.* must be used
  
  ### 2 | Cloning the repo 
  __clone this the repo to your local machine__
  
  ```
    git clone https://github.com/MULUALEM-TEKLE/trada.git
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
