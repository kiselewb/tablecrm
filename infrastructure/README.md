<h1 align="center">Tablecrm Infrastructure</h1>

## Как пользоваться?
* Скопируйте .env.example в тот же каталог с именем .env:
```
cp ./.env.example ./.env
```
* Запустите контейнеры:
```
docker compose up -d --build
```

## FAQ
* Если возникли проблемы с портами, узнайте, какой процесс занимает данный порт:
```
sudo lsof -i :port
```
и убейте этот процесс, если это необходимо:
```
sudo kill PID
```
* Иначе измените порт в конфигурационном файле docker-compose.yml и в configuratuin/nginx/template.conf