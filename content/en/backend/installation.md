---
title: Installation
category: Backend
description: 'Laravel backend up and running with docker'
position: 1
---

## Requirements
 - Docker
 - Git

##  Before Install

### Clone repo
```bash
  git clone git@gitlab.com:seelo/pomodoro/backend.git
```

### Verify ports
Make sure you have nothing running on the following ports
otherwise change or add the Env variable into your `.env` with a different 
port, so you do not have conflicts.

| Name        | Default Port | Env Variable                   |
|-------------|:-------------|:-------------------------------|
| Laravel     | `80`         | APP_PORT                       |
| Mysql       | `3306`       | FORWARD_DB_PORT                |
| Mailhug     | `1025`       | FORWARD_MAILHOG_PORT           |
| Mailhug     | `8025`       | FORWARD_MAILHOG_DASHBOARD_PORT |

##  Install

### Generate the .env file

```bash
cp .env.example .env
```

### Laravel Sails
instead of repeatedly typing vendor/bin/sail to execute Sail commands,
you may wish to configure a Bash alias that allows you to execute Sail's
commands more easily:

```bash
alias sail='bash vendor/bin/sail'
```

Once the Bash alias has been configured, you may execute Sail 
commands by simply typing sail. 
```bash
sail up
```

### Start containers and server
  ```bash
cd ./backend
sail up
sail artisan migrate
  ```


For more information about sail command refer to 
[laravel Sails](https://laravel.com/docs/8.x/sail)


#### Expose server:
```bash
./vendor/bin/sail share --subdomain=pomodoro
or 
php artisan expose
```

### Up and running
Now that all is installed you can access the application via:

| Name        | Url                                 | Description                 |
|:------------|:------------------------------------|:----------------------------|
| Laravel     | http://localhost:80                 | Main laravel application    |
| Mailhug     | http://localhost:8025               | Local email testing         |



## Database connection

These are de default values
you can change them in your `.env` file

|  Name     |  Value     |
|:----------|:-----------|
| Host      | `0.0.0.0`  |
| port      | `3306`     |
| database  | `backend`  |
| username  | `sail`     |
| password  | `password` |
