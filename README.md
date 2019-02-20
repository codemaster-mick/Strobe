# Strobe
Dockerized LAMP stack for ultra rapid deployment

## Internal server versions
 - Apache 2
 - MariaDB 10.1.38
 - PHP 7.2.14

## Getting started
```
git clone https://github.com/codemaster-mick/Strobe.git
cd Strobe
docker-compose up
```

Wait a minute or two for everything to finish spinning up then open your browser to your freshly deployed [LAMP stack](http://localhost/index.html).

## Next steps

Once everything has loaded, you can use Ctrl+C to stop docker-compose and restart the containers however you normally manage your Docker containers. From this point on, so long as the stack is running, anything placed inside the DocumentRoot directory will immediately be served by Apache.

### Manually starting the stack
Should you need to start the stack manually, run the following commands (IN ORDER!)
```
docker start lampstack-mariadb
docker start lampstack-apache
docker start lampstack-phpmyadmin
```
