# Made.com PHPCS Magento Rules

A set of [http://pear.php.net/package/PHP_CodeSniffer](PHPCS) rules used by
made.com when hacking Magento.

## Pre-Requisites

* [PHPCS](http://pear.php.net/package/PHP_CodeSniffer)

## Installation

### Short Version

Clone this repository into your PHPCS Standards directory, using the directory
name of `Made`

### Long Version

You need to know the directory of your PHPCS install, you can do this by opening
a command prompt and typing in the following:

    pear list-files PHP_CodeSniffer

You should see a load of lines looking like this:

    php    /usr/share/php/PHP/CodeSniffer/Reporting.php
    php    /usr/share/php/PHP/CodeSniffer/Sniff.php
    php    /usr/share/php/PHP/CodeSniffer/Tokens.php

So the PHPCS directory in this case is `/usr/share/php/PHP/CodeSniffer/`, so we
need to [download](https://github.com/madedotcom/phpcs-magento-rules/zipball/master)
or clone this repository into this directory:

    /usr/share/php/PHP/CodeSniffer/Standards/Made

You can check the standard got installed by running `phpcs -i` which should show
you something like this:

    The installed coding standards are MySource, Squiz, Zend, PHPCS, Made and PEAR