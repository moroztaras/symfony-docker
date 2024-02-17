# Symfony docker example

Project on Symfony 6 using docker(php-fpm, nginx, postgres).

## Install project

### Things you need
* composer
* npm
* docker

### Clone repository to your local machine
```bash
git clone git@github.com:moroztaras/symfony-docker.git
```

### Create project config
```bash
cd symfony-docker
cp docker/.env.dist docker/.env
```

### Build a project in the docker
```bash
make build
```

### Run a project with the docker
```bash
make up
```
### Go inside the container
```bash
make app_bash
```

### Create new Symfony project
```bash
composer create-project symfony/skeleton:"6.2.*" app
```

### Exit from container 
```bash
exit
```
Move file from directory ./app to . and delete empty directory /app

### Crate env file 
It's credentials to database.
```bash
cp env .env.local
```

### Go to the link at
```bash
http://127.0.0.1:888
```

© 2024