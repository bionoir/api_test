# api_test

Here some useful commands

> composer create-project symfony/skeleton <NOM_PROJET>
> cd <NOM_PROJET>
> composer req api

## modifier le fichier '.env' pour paramétrer la base de données

> php bin/console doctrine:database:create

> php bin/console doctrine:schema:update

> composer req symfony/maker-bundle --dev 

> php bin/console make:entity
	==> répondre aux questions
	
> php -S localhost:8000 -t public

## aller dans localhost:8000/api

## avec PHP 8.0 à jour (composer.json) ajouter dans l'entité l'annotation #[ApiResource] la ligne avant le nom de la classe

## préparation base de données

> php bin/console make:migration

> php bin/console doctrine:migrations:migrate

## ajouter/modifier les entités avec "php bin/console make:entity"

## ensuite faire:

> php bin/console make:migration
> php bin/console doctrine:migrations:migrate
