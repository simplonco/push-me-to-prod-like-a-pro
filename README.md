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

## Step 2 - Generate a Symfony App

TODO..

## Step 3 - Push to Prod - the Heroku way

Try to deploy your app on heroku, that's simple and free:
https://devcenter.heroku.com/articles/getting-started-with-symfony	

e.g: https://is-it-raining-today.herokuapp.com/?q=Paris !

[![Heroku](https://d3k90kvix375hb.cloudfront.net/assets/heroku-og-cad174838a49b266550809e29026ec9bc18e056dae8f9cf523ea4237379691f9.png)](https://heroku.com/)
