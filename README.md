# PostgresPro 11.4.1 in Docker

## Порядок установки

1. Устанавливаем Docker (Docker Desktop для Windows или Docker для Linux)

2. Собираем образ: `docker build -t ImageName ./`, например: `docker build -t pgpro_11.4.1 ./`

3. Указываем `ImageName` в docker-compose.yml, например: `image: pgpro_11.4.1:latest`

4. Компонуем контейнер: `docker compose up -d`
