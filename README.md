# Coding Standards

This repository is intended to contain settings files for different editors etc to assist developers working on OpenEyes code to adhere to the Coding Standards. It's hoped that users of different editors will export the settings they use to contribute to this repository.

Settings files should be added to the settings directory.

## PHP

* Code should adhere to the MUST clauses of the [PSR-2](http://www.php-fig.org/psr/psr-2/) guidelines.
* Code should be documented using [PHPDoc](http://www.phpdoc.org/).  
* Where possible in the development of event type modules, call methods on inherited core code rather than reinventing things.  We will continue to improve these available methods
* Variable names. Variables should be named with underscores **not** camelCase. 

The main modules and core code have been checked by PHP CS code fixer to make sure everything is [PSR-2](http://www.php-fig.org/psr/psr-2/) compliant however there are still many inconsistencies in the code in regard to style, particularly with the naming of variables and tab indentation in views. All new code should follow the guidelines, old code should be updated when convenient.

**If you do re-format code, please ensure the change is committed separately from any functional change.**

_**Note** In the past, the standard has been to indent code with tabs, but this inconsistency with the PSR-2 standards makes little sense. As such, all new code should be indented with spaces as per PSR-2. Where old code has not been corrected yet, please follow the old indentation approach._

## HTML

* As far as possible we are aiming at HTML5 compliance.  
* The Moorfields implementation is currently targeted at and tested against webkit (Recent versions of Chrome and Safari) as this is what we are deployed to because of our need for a strong HTML5 implementation for EyeDraw.

## JavaScript

* Avoid relying on DOM selectors which may be fragile (e.g. an element's relative position). 
* There should be a distinction between CSS classes which are used for control (javascript) and styling. 
