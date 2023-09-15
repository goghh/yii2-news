Copy .env

    cp .env.example .env

Copy frontend .env

    cd frontend
    cp .env.example .env
    cp ..

Change runtime folder permissions

    sudo chmod 777 -R runtime

Start the container

    docker-compose up -d --build

Install vendor packages

    docker-compose run --rm php composer install

Run migrations

    docker-compose run --rm php yii migrate

Open

    http://localhost:3000/
