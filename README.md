# Private Docker Registry

Sets up a private docker registry on a docker server.

## Setup Local Development

1. Clone the repository.
2. In a terminal, navigate to the auth folder and run `htpasswd -Bc registry.password <username>`. Fill out the password.
    - Requires apache2-utils is installed on Ubuntu
3. Run the docker with docker-compose `docker-compose up -d`.