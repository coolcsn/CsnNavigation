CsnNavigation
=======

**What is CsnNavigation?**

CsnNavigation is a Module for Navigation based on Zend Framework 2

**What exactly does CsnNavigation?**

CsnNavigation has been created with educational purposes to demonstrate how Navigation can be done. It is fully functional.

Installation
============

Installation via composer is supported, just make sure you've set ```"minimum-stability": "dev"```
in your ```composer.json```file and after that run ```php composer.phar require coolcsn/csn-navigation:dev-master```

Go to your application configuration in ```./config/application.config.php```and add 'CsnNavigation'.
An example application configuration could look like the following:

```
'modules' => array(
    'Application',
    'CsnNavigation'
)
```

Navigation configuration
=============

Copy `./vendor/coolcsn/csn-navigation/config/navigation.global.php.dist` to
   `./config/autoload/navigation.global.php` and edit.

Show navigation
=============
Add this somewhere in your layout `./module/Application/view/layout/layout.phtml` :
```
<?php echo $this->navigation('navigation')->menu(); ?>
```

Recommends
==========
CsnUser - Authentication (login, registration) module, fully compatible with CsnAuthorization.

CsnAuthorization - Authorization compatible for this Registration and Logging;

CsnCms - Content management system;