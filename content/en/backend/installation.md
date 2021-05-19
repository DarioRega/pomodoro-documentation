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
| Meilisearch | `7700`       | FORWARD_MEILISEARCH_PORT       |
| Redis       | `6379`       | FORWARD_REDIS_PORT             |

##  Install
  ```bash
  cd ./backend
  ./vendor/bin/sail up
  ```
