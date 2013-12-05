# PHPWord

This repository is an source code of [PHPWord](http://phpword.codeplex.com/), turned into a [Composer](http://getcomposer.org/) package.
I cloned this from [kkula](https://bitbucket.org/kkula/phpword/) and made some changes to make it work with [Symfony2](http://symfony.com).

## Perquisites:

 * PHP 5.2.x or newer
 * PHP Extension ZipArchive
 * PHP Extension xmllib

## Installation
All you have to do is to [get composer](http://getcomposer.org/download/) and add following lines to your `composer.json`:

        "require": {
            //...
           "ferdynator/phpword": "v1.0"
        }

### Add as service (optional):

In your `services.xml`:

        <service id="PHPWord" class="PHPWord">
            <file>%kernel.root_dir%/../vendor/ferdynator/phpword/Library/PHPWord.php</file>
        </service>
