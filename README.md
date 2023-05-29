# ИДЗ-4
# Шаламкова Алиса БПИ-218

### Запуск программы:
```
go run ./auth/cmd/main.go
```
```
go run ./order/cmd/main.go
```

При логине пользователю в куки сохраняется jwt токен, 
при последующих запросах токен вычитывается из куки, а из токена расшифровываются id, username, role

Запросы в сервис order (кроме получения меню) может отправлять только авторизованный пользователь.
Все конечные точки и примеры запросов экспортированы в коллекцию Postman,
коллекцию можно импортировать с помощью файла kpo.postman_collection.json