# localhost_api
 
Нагружаем локальное API. Порядок действий для быстрой установки.
1. В папке где будет лежать наше api выполнить:
npm init -y
В результате получаем package.json
2. В этой же папке устанавливаем json-server:
npm install json-server
3. В package.json (созданный в первом пункте) добавляем скрипт для старта json-сервера:
"scripts":{
    "start": "json-server db.json"
  }
4. Сохраняем и запускаем в терминале:
npm start
Должно подняться на 3000 порту локалхоста:

> localhost_api@1.0.0 start D:\projects\performance_testing\localhost_api
> json-server db.json


  \{^_^}/ hi!

  Loading db.json
  Done

  Resources
  http://localhost:3000/users

  Home
  http://localhost:3000

  Type s + enter at any time to create a snapshot of the database
При открытии http://localhost:3000/users в терминале логируется запрос например - GET /users 200 31.448 ms - 115.
5. Открываем LOCAL_API_TEST.jmx и экспериментируем.
