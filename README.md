
Запускаем rabbit и kafka
```
docker-compose up -d
```

Инициализируем rabbit
```
./rabbit_schema_initialize.sh
```

Инициализируем kafka
```
./kafka_schema_initialize.sh
```

Запускаем приложение
```
mvn clean package
mvn spring-boot:run
```

пробуем отправить что-то в rabbit и kafka через наше приложение