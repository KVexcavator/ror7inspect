$ docker build .
$ docker images
$ docker tag 6ed572358c60 ror7inspect
$ docker build -t ror7inspect .
$ docker run -p 3000:3000 ror7inspect
===============================
sudo chown excavator:excavator -R docker-app/
===============================
Generate a Gemfile.lock:
docker run --rm -v "$PWD":/usr/src/app -w /usr/src/app ruby:3.2 bundle install
===============================
$ docker compose up --build
$ docker compose exec ror7 bin/rails g model User username

$ docker compose exec ror7 bin/rails importmap:install
$ docker compose exec ror7 bin/rails turbo:install
$ docker compose exec ror7 bin/rails turbo:install:redis

docker compose exec ror7 bin/rails g model Message user:references room:references content:text
