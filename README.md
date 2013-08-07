CsnNavigation
=======

**What is CsnNavigation?**

CsnNavigation is a Module for Navigation based on Zend Framework 2

**What exactly does CsnNavigation?**

CsnNavigation has been created with educational purposes to demonstrate how Navigation can be done. It is fully functional.

Installation
============

Installation via composer is supported, simply add the following line to your ```composer.json```

```
"repositories": [
	{
		"type": "vcs",
		"url": "https://github.com/coolcsn/CsnNavigation"
	}
],
"require" : {
    "coolcsn/csn-navigation": "dev-master"
}
```

After adding to the composer's packagist.org (not ready yet)

```
"require" : {
    "coolcsn/csn-navigation": "dev-master"
}
```

An example application configuration could look like the following:

```
'modules' => array(
    'Application',
    'CsnNavigation'
)
```

Navigation configuration
=============

Copy `./vendor/coolcsn/csn-navigation/data/navigation.global.php.dist` to
   `./config/autoload/navigation.global.php` and edit.

Show navigation
=============
Add this somewhere in your layout / view script:
```
<?php echo $this->navigation('navigation')->menu(); ?>
```