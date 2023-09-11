# NativePHP PoC

Just wanted to try out the new (as of September 2023) NativePHP implementation. 

Steps i had to take to get it running:

* create a new laravel application with ```composer create-project laravel/laravel projectname```
* next install the nativephp dependencies ```composer require nativephp/electron```
* integrate these libs with laravel ```php artisan native:install```
* run the application dev server with ```php artisan native:serve```

If you get messages that some shared libraries are missing, install them with ```apt``` e.g.:
```bash
sudo apt update 
sudo apt install libnss3-dev libgdk-pixbuf2.0-dev libgtk-3-dev libxss-dev libasound2
```

(These were the libraries that were missing on my WSL Ubuntu 22 installation). 

Enjoy!