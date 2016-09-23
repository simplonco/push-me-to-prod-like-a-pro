Push to production like a PRO!
===============

_Learn how to put a real app online_

![Indiana Jones](indiana-jones.gif)

## Step 1 - Install Composer

```shell
php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
php -r "if (hash_file('SHA384', 'composer-setup.php') === 'e115a8dc7871f15d853148a7fbac7da27d6c0030b848d9b3dc09e2a0388afed865e6a3d6b3c0fad45c48e2b5fc1196ae') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
php composer-setup.php
php -r "unlink('composer-setup.php');"

sudo mv composer.phar /usr/local/bin/composer
```

## Step 2 - Generate a Composer config

* for a simple PHP project:

```shell
composer init
```

* for a Symfony app:

```shell
composer create-project "symfony/framework-standard-edition:^3.0" new-symfony-project
```

* Learn more about:

http://boulogne.simplon.co/wp-content/uploads/2016/03/Tutoriel-PHP-Composer.pdf

## Step 3 - Push to Prod - the Heroku way

Try to deploy your app on heroku, that's simple and free!

Start by following the guide **Getting Started on Heroku with PHP**:
https://devcenter.heroku.com/articles/getting-started-with-php
_TODO.._

Next, read the **Getting Started with Symfony on Heroku** tutorial:
https://devcenter.heroku.com/articles/getting-started-with-symfony	

Basically you have to do:
```
# Run this from your terminal:
# Please ensure that you have Ruby installed.
wget -qO- https://toolbelt.heroku.com/install.sh | sh
# Create an Heroku instance
heroku create
# If you use Symfony set env to PROD
heroku config:set SYMFONY_ENV=prod
# Push to PROD
git push heroku master
```

At the end, you will get your app online, e.g:
- https://galactic-space-combat.herokuapp.com/
- https://is-it-raining-today.herokuapp.com/?q=Paris

[![Heroku](https://d3k90kvix375hb.cloudfront.net/assets/heroku-og-cad174838a49b266550809e29026ec9bc18e056dae8f9cf523ea4237379691f9.png)](https://heroku.com/)
