# docker-mysql
Comando para criação de um container com banco de dados MYSQL com o uso do docker

 docker container run --name desafio02 -d -p 3306:3306 -e MYSQL_DATABASE=docker_db -e MYSQL_USER=docker_usr -e MYSQL_PASSWORD=docker_pwd -e MYSQL_ROOT_PASSWORD="docker admin" mysql

docker container run <-- é usado para criação de um container em cima de uma imagem 
-- name NOME <-- é usado para escolher o nome do container o nome dele ser colocado logo em seguida 
-d <-- mostra para o Deamon que o container é um teste e deve ser continuo 
-p 5000:5400 <-- é para escolher a porta de saido do container 5000: é a porta e 5400 é a subporta (Modificado somente para o exemplo) 
-e <-- é usado para podermos adicionar as variaveis da imagem e devem sempre estar antes da variavel 
mysql <-- e o nome da imagem e sempre deve estar no final. 
-e MYSQL_DATABASE=NOMEDOBANCO 
-e MYSQL_USER=NOMEDOUSUARIO 
-e MYSQL_PASSWORD=SENHADOBANCO
