# 20200902
#Utilização do Docker Laradock (Laradock é um ambiente de desenvolvimento PHP completo para Docker.)

1 - Clone Laradock dentro do seu projeto PHP:
git clone https://github.com/Laradock/laradock.git

2 - Entre na pasta laradock e renomeie env-example para .env.
cp env-example .env

3 - Execute seus contêineres:
docker-compose up -d nginx mysql phpmyadmin redis workspace 

4 - Abra o .env arquivo do seu projeto e defina o seguinte:

DB_HOST=mysql
REDIS_HOST=redis
QUEUE_HOST=beanstalkd
5 - Abra seu navegador e visita localhost: http://localhost.
