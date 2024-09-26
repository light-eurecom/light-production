# Light production

Make sure to properly clone this git project, using `--recurse-submodules` as this repository references other child repositories.

```bash
git clone --recurse-submodules https://github.com/light-eurecom/light-production.git
```

## Prepare backend

`cd light-core` and create the environment file:

```bash
cp env.example env.production
```

Update it accordingly:

```bash
FLASK_ENV=production
SECRET_KEY=my_secret
LIGHT_HOST="https://light.eurecom.fr"
```

Update it accordingly:

```bash
FLASK_ENV=production
SECRET_KEY=my_secret
LIGHT_HOST="https://light.eurecom.fr"
```

## Run docker-compose

Then `cd light-production` and run:

```bash
sudo docker-compose up -d
```
