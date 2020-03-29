# Private Docker Registry

Sets up a private docker registry on a docker server.

## Setup Local Development

1. Clone the repository.
2. In a terminal, navigate to the auth folder and run `htpasswd -Bc registry.password <username>`. Fill out the password.
    - Requires apache2-utils is installed on Ubuntu
3. Run the docker with docker-compose `docker-compose up -d`.

## Setup Production

1. Clone the repository.
2. Copy .env-dist to .env and fill out the REGISTRY_URL with the public url for the registry.
3. In a terminal, navigate to the auth folder and run `htpasswd -Bc registry.password <username>`. Fill out the password.
    - Requires apache2-utils is installed on Ubuntu
4. Run the docker with docker-compose `docker-compose -f docker-compose.yml -f docker-compose.prod.yml up -d`.