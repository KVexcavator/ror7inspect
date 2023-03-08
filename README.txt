$ docker build .
$ docker images
$ docker tag 6ed572358c60 ror7inspect
$ docker build -t ror7inspect .
$ docker run -p 3000:3000 ror7inspect
===============================
sudo chown excavator:excavator -R docker-app/
===============================
$ docker compose up --build
$ docker-compose exec ror7 bin/rails g model User username
