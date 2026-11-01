# ACLClouds Auto Renew

Ежедневно проверяет бесплатный сервис ACLClouds и пытается продлить его, когда открывается окно продления.

## Настройка

В GitHub откройте **Settings → Secrets and variables → Actions** и добавьте Secrets:

- `ACL_USERNAME` — логин первого ACLClouds-аккаунта;
- `ACL_PASSWORD` — пароль первого ACLClouds-аккаунта;
- `ACL_SERVER_ID` — необязательно; если оставить пустым, скрипт попробует найти сервис сам.

Не отправляйте эти значения в чат и не добавляйте их в файлы репозитория.

Workflow запускается ежедневно в 03:17 UTC и вручную через **Actions → ACLClouds Auto Renew → Run workflow**.

Переменная репозитория `ACL_BASE_URL` необязательна и по умолчанию равна `https://aclclouds.com`.
