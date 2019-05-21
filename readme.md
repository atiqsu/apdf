## PDF Manager

### How to create package

- Create a Github repository
- Checkout it in your Laptop/PC
- Create readme.md file [optional]
- Create .gitignore file [optional]
- Create composer.json file Or run 'composer init' command from terminal inside the project folder
    - Put name as the repo name with username like `gitusername/repo`
    - Put stability as stable
- Create a folder named `src`
- Now Add the following into composer.json file :
```shell
"autoload": {
        "psr-4": {
            "Atiq\\APDF\\": "src/"
        }
    }
```    
- Change the namespace `Atiq\\APDF\\` into whatever you like



## Installation

Require this package with composer:

```shell
composer require barryvdh/laravel-debugbar
```

After updating composer, add the ServiceProvider to the providers array in config/app.php

> If you use a catch-all/fallback route, make sure you load the Debugbar ServiceProvider before your own App ServiceProviders.

