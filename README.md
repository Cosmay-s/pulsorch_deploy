# deploy

стоп всех контейнеров
 docker stop -t1 $(docker ps -aq)

 # Полная пересборка
docker compose down -v
docker compose build
docker compose up -d

# Проверка логов
docker compose logs -f api
 
