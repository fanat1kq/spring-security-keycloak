1 запустить docker compose
2 создать реалм
3 создать клиент с аутентификацией (можно указать разные гранты) !доразобраться
4 создать пользователя с обязальным указанием логина, пароля, почты+varyfed, фио
5 указать секрет клиента в yml
6 уже можно получить токен по url по пост методу с указанием в теле необходимых полей
7 добавить роль и привязать к пользователю
8 Добавить маппинг User Realm Role в скоупах клиента и в jwt добавиться claim "User Realm Role"
           var roles = (List<String>) jwt.getClaimAsMap("realm_access").get("roles"); - до маппинга
