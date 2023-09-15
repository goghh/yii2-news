Copy .env

    cp .env.example .env

Copy frontend .env

    cd frontend
    cp .env.example .env

Start the container

    docker-compose up -d --build

Install vendor packages

    docker-compose run --rm php composer install

Run migrations

    docker-compose run --rm php yii migrate

Open

    http://localhost:3000/
