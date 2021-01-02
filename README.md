# Présentation du projet
C'est notre 2ème projet. L'objectif étant la réalisation, par équipe, d'un site dynamique sur une durée de 6 semaines. Le thème étant la création d'un site permettant à notre professeur de regrouper l'ensemble des projets réalisés par les élèves de la Wild, afin de pouvoir les présenter à des etreprises pour de futurs collaborations. Ce site a été déployé.
Notre groupe a utilisé une architecture simple MVC et les langages suivants:
  * HTML / CSS / Javascript
  * PHP
  
Notre site possède les fonctionnalités suivantes:
  * Navbar permettant d'accéder directement à un type de projet, barre de recherche, connexion pour la partie administrateur.
  * Affichage des différents projets sur la page d'accueil avec tri par type de projet.
  * Footer permettant d'avoir les coordonnées de notre professeur et école pour plus de renseignements.
  * Une page de détails de présentation d'un projet, avec images des pages du projet, le type de projet, année, type de langage, description.
  * une barre de recherche permettant de chercher un mot dans le titre ou dans le descriptif.
  * une connexion sécurisée vers la partie administrateur.
  * Possibilité pour l'administrateur d'ajouter, de modifier, supprimer un projet. 

Possibilité de visualisé un aperçu du site dans l'onglet Wiki.-> https://github.com/Angelus-Dev-GitHub/Project2_WildProjects/wiki






# Simple MVC

## Description

This repository is a simple PHP MVC structure from scratch.

It uses some cool vendors/libraries such as Twig and Grumphp.
For this one, just a simple example where users can choose one of their databases and see tables in it.

## Steps

1. Clone the repo from Github.
2. Run `composer install`.
3. Create *config/db.php* from *config/db.php.dist* file and add your DB parameters. Don't delete the *.dist* file, it must be kept.
```php
define('APP_DB_HOST', 'your_db_host');
define('APP_DB_NAME', 'your_db_name');
define('APP_DB_USER', 'your_db_user_wich_is_not_root');
define('APP_DB_PWD', 'your_db_password');
```
4. Import `simple-mvc.sql` in your SQL server,
5. Run the internal PHP webserver with `php -S localhost:8000 -t public/`. The option `-t` with `public` as parameter means your localhost will target the `/public` folder.
6. Go to `localhost:8000` with your favorite browser.
7. From this starter kit, create your own web application.

### Windows Users

If you develop on Windows, you should edit you git configuration to change your end of line rules with this command :

`git config --global core.autocrlf true`

## URLs availables

* Home page at [localhost:8000/](localhost:8000/)
* Items list at [localhost:8000/item/index](localhost:8000/item/index)
* Item details [localhost:8000/item/index/show/:id](localhost:8000/item/show/2)
* Item edit [localhost:8000/item/index/edit/:id](localhost:8000/item/edit/2)
* Item add [localhost:8000/item/index/add](localhost:8000/item/add)
* Item deletion [localhost:8000/item/index/delete/:id](localhost:8000/item/delete/2)

## How does URL routing work ?

![Simple MVC.png](https://raw.githubusercontent.com/WildCodeSchool/simple-mvc/master/Simple%20-%20MVC.png)
