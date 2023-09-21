# Wordpress Docker Setup
Ce projet fournit une configuration Docker simple pour démarrer rapidement avec WordPress, MySQL et phpMyAdmin.

# Prérequis
Docker
Docker-Compose

# Installation

# Clonez ce dépôt :
git clone https://github.com/wllmz/wordpress-docker.git
cd wordpress-docker

# Configuration avec .env
Avant de démarrer les conteneurs, vous pouvez personnaliser certains paramètres en modifiant le fichier .env. Ce fichier contient des variables d'environnement utilisées par Docker Compose.
Exemple de contenu du fichier .env :

WORDPRESS_DB_HOST=db
WORDPRESS_DB_USER=exampleuser
WORDPRESS_DB_PASSWORD=examplepass
WORDPRESS_DB_NAME=exampledb
MYSQL_DATABASE=exampledb
MYSQL_USER=exampleuser
MYSQL_PASSWORD=examplepass
MYSQL_RANDOM_ROOT_PASSWORD=1
PMA_HOST=db
MYSQL_ROOT_PASSWORD=examplepass

# Lancez les conteneurs Docker :
docker-compose up -d

# Accédez à WordPress :
Ouvrez votre navigateur et allez à http://localhost:8080.

# Accédez à phpMyAdmin :
Ouvrez votre navigateur et allez à http://localhost:8081.

