# Домашнее задание к занятию "Работа с данными (DDL/DML)" - Перугнов Д.В

### Задание 1
1.Установили MySQL используя Docker контейнер  
![image](https://github.com/dimindrol/12-02-DDL-DML/assets/103885836/7a3da180-5ff9-4c5b-87ec-e1d77b64f013)  
2. Подключились к БД используя Dbeaver  
![image](https://github.com/dimindrol/12-02-DDL-DML/assets/103885836/95eb8916-ce65-40d3-9bbd-2b03b6d03444)   
3.Создали нового пользователя  
```sql
CREATE USER 'sys_temp'@'localhost' IDENTIFIED BY "password";
```
![image](https://github.com/dimindrol/12-02-DDL-DML/assets/103885836/e27eb60b-1af1-4fc5-b59a-5e0a18e8cc61)  
4. Просмотр всех пользователей
```sql
SELECT user FROM mysql.user
```
![image](https://github.com/dimindrol/12-02-DDL-DML/assets/103885836/41879eed-996f-4004-8508-8efebdcd95e2)  
5.Предоставление всех прав пользователю sys_temp
```sql
GRANT ALL PRIVILEGES ON *.* TO 'sys_temp'@'localhost';
```
![image](https://github.com/dimindrol/12-02-DDL-DML/assets/103885836/b088a47a-8a60-4e66-b2f5-976426af6e42)  
6. Запрос на получение списка прав для пользователя  
```sql
SHOW GRANTS FOR 'sys_temp'@'localhost';
```
![image](https://github.com/dimindrol/12-02-DDL-DML/assets/103885836/d7cf378a-5f79-4c25-a8d4-b06c49de8eec)
7. Переподключились к БД от имени sys_temp
![image](https://github.com/dimindrol/12-02-DDL-DML/assets/103885836/b0158b7a-c988-4ed3-b345-ee3b80542559)  
8.Восстановили дамп в базу данных, сформировали ER-диаграмму
![image](https://github.com/dimindrol/12-02-DDL-DML/assets/103885836/1be8a43e-dc51-40db-a91a-85cbcc8ff9c1)

### Задание 2
Сопоставление таблицы и первичного ключа
![image](https://github.com/dimindrol/12-02-DDL-DML/assets/103885836/e5bc5d5a-a4c6-417b-8c9f-6a07b79db5da)











