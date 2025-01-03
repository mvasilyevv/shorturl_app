# shorturl_app

---

## Запуск через Docker с помощью docker-compose
1. Убедитесь, что у вас установлены **Docker**.
2. Откройте файл [docker-compose.yml](docker-compose.yml).
3. В консоли (в корне проекта) выполните команду:
   ```bash
   docker-compose up -d
4. По завершении сборки и запуска контейнеров приложение будет доступно по адресу, указанному в разделе **ports** файла docker-compose.yml.
5. Например, если указан порт 8081:80, то нужно открыть в браузере:
    ```commandline
    http://localhost:8081/docs
   
## Запуск локально (без Docker)
1. Убедитесь, что у вас установлен Python 3.9+ и pip.
2. Установите зависимости:
    ```bash
    pip install -r requirements.txt
3. Запустите сервер:
    ```bash
   uvicorn main:app --host 0.0.0.0 --port 8081
4. После запуска приложение будет доступно по адресу:
    ```commandline
    http://localhost:8081/docs
