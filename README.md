# Развертывание API для YaMDb в docker. 

Проект на Django rest framework, база отзывов о фильмах, книгах и музыке.

## Установка docker

Проверяем установлен ли docker
```
docker -v
```
и docker-compose
```
docker-compose -v
```
Если не установлен, скачиваем с сайта [docker.com](https://www.docker.com/), следуя инструкциям для вашей ОС.

### Запуск контейнера

Сборка контейнера
```
docker-compose up
```
Для входа в контейнер выполните команду
```
docker-compose exec web bash
```
Выполняем миграцию базы данных
```
python3 manage.py migrate
```
Создаем суперпользователя
```
python3 manage.py createsuperuser
```
