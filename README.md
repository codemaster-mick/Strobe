# Strobe
Dockerized LAMP stack for ultra rapid deployment

## Internal server versions
- Apache 2
- MariaDB 10.1.38
- PHP 7.2.14

## Features
- Highly configurable
- Comes with helper scripts
- Automatic phpMyAdmin login

## Getting started
```
git clone https://github.com/codemaster-mick/Strobe.git
cd Strobe
```
Now adjust the .env file to represent what you would like your instance to look like and then run
```
docker-compose up
```
to get the stack building.

Wait a minute or two for everything to finish spinning up then open your browser to your freshly deployed [DAMP stack](http://localhost/index.html) (Docker Apache Maria PHP).

## Next steps

Once everything has loaded, you can use Ctrl+C to stop docker-compose and restart the containers however you normally manage your Docker containers. From this point on, so long as the stack is running, anything placed inside the DocumentRoot directory will immediately be served by Apache.

### Manually starting the stack
Should you need to start the stack manually, run the following commands (IN ORDER!)
```
docker start lampstack-mariadb
docker start lampstack-apache
docker start lampstack-phpmyadmin
```
