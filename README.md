# PostgresPro 11.4.1 in Docker

## Порядок установки

1. Устанавливаем Docker (Docker Desktop для Windows или Docker для Linux)

2. Собираем образ: `docker build -t ImageName ./`, например: `docker build -t pgpro_11.4.1 ./`

3. Вместо сборки образа его можно скачать c https://hub.docker.com: `docker pull romanstarch/pgpro_11.4.1:latest`

4. Указываем `ImageName` в docker-compose.yml, например: `image: pgpro_11.4.1:latest` (или `image: romanstarch/pgpro_11.4.1:latest`)

5. Компонуем контейнер:
    - `docker compose up -d` (команда для Windows)
    - `docker-compose up -d` (команда для linux, потребуется предварительная установка утилиты docker-compose, а также изменить тег `version` в docker-compose.yml: `version: "3.3"`)

### Примечание

Сервер postgres собран с языковыми настройками: `ru_RU.UTF-8`
