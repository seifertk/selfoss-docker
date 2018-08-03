# Selfoss Docker
A container that runs selfoss.

`docker-compose up` for selfoss + nginx or `docker build ./app -t selfoss`

Make `/var/data` a volume for persistence.

See https://selfoss.aditu.de/ for configuration. 
Use environment variables, e.g. "selfoss_username".
Or use an environment file with docker compose, like .env.example
