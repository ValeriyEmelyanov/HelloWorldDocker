### Цель проекта
Показать запуск простого консольного приложения Java в контейнере Docker.

### Работа с Docker

Создать образ (просто Hello world)
```
docker build -t hello-world:1.0 .
```
Посмотреть список образов
```
docker images
```
Создать контейнер и запустить
```
docker run hello-world:1.0
```

Создать образ (с бесконечным циклом)
```
docker build -t hello-world:2.0 .
```
Создать контейнер и запустить в фоне (открепленный режим / другой процесс)
```
docker run -d hello-world:2.0
```
Посмотреть список запущенных процессов / контейнеров (подсмотреть ID процесса)
```
docker ps
```
Посмотреть лог процесса / контейнера по ID
```
docker logs 2c505e438bad
```
Остановить процесс / контейнер по ID
```
docker stop 2c505e438bad
```
Посмотреть список всех контейнеров
```
docker ps -a
```
Удалить контейнер по ID
```
docker rm 2c505e438bad
``` 

### Полезные ссылки
* [Getting Started with Docker](https://www.youtube.com/watch?v=FzwIs2jMESM&list=PLPZy-hmwOdEXZ7m_3JtanruRUhaAuI_uh)
