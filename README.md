# Conquest


This is a Yii2 application.

## Installation

1. Install composer

2. Install composer-asset-plugin needed for yii assets management
```bash
composer global require "fxp/composer-asset-plugin"
```

3. Clone the repository
```
git clone https://github.com/shadyueh/conquest.git conquest
```

4. Install composer dependencies
```
composer install
```

### Setup application
1. Copy `.env.dist` to `.env` in the project root.
2. Adjust settings in `.env` file
  - Set debug mode and your current environment
  ```
  YII_DEBUG   = true
  YII_ENV     = dev
  ```
  - Set DB configuration
  ```
  DB_DSN           = mysql:host=127.0.0.1;port=3306;dbname=conqdb
  DB_USERNAME      = user
  DB_PASSWORD      = password
  ```

  - Set application canonical urls
  ```
  FRONTEND_URL    = /
  BACKEND_URL     = /admin
  STORAGE_URL     = /storage/web
  ```

4. Run in command line
```
php console/yii app/setup
```

5. Configure a virtual host