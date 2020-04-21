# TDD Project

## Installation 
Positionnez votre terminal à la racine de votre projet et tapez la commande :
  
> git clone https://github.com/Cyrhades/TDD_hotel ./tests

Modifiez la ligne 3 du fichier ./tests/phpunit.xml en donnant le nom du namespace de votre Framework dans l'attribut "value".
Si nécessaire modifiez la ligne 4 du fichier ./tests/phpunit.xml en donnant le port que vous utilisez pour votre serveur HTTP dans l'attribut "value".



## Usage
Pour lancer vos tests tapez la commande en étant placé à la racine de votre projet:

- Lancer les tests de votre serveur HTTP
> ./vendor/bin/phpunit -c tests/phpunit.xml --testsuite server

- Lancer les tests concernant la connexion à Mongodb pour les fixtures
> ./vendor/bin/phpunit -c tests/phpunit.xml --testsuite fixtures-server

- Lancer les tests concernant les fixtures customers
> ./vendor/bin/phpunit -c tests/phpunit.xml --testsuite fixtures-customers

- Lancer les tests concernant les fixtures rooms
> ./vendor/bin/phpunit -c tests/phpunit.xml --testsuite fixtures-rooms

- Lancer l'ensemble des tests des fixtures
> ./vendor/bin/phpunit -c tests/phpunit.xml --testsuite fixtures
