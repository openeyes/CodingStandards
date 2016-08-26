# PHPStorm Setup

To import the settings, load it through:

File -> Import Settings...

After you have restarted, you will need to setup phpmd and phpcs. The following assumes you are working with the OpenEyes main repository, and have already run ```composer install```

## PHPmd

Open ```Preferences``` from the main menu. 

For convenience, it is easier to search for Mess Detector as this will bring up the two settings you need to configure

### Languages and Frameworks

Here is where you setup PHPStorm to point to the right command line script for mess detection. On Configuration, click the ```...``` to bring up the finder window. Select ```openeyes/bin/phpmd```

### Editor -> Inspections

You need to select the custom rulesset which is included with OpenEyes. Click the plus button under Custom Ruleset, and select ```openeyes/build/phpmd```

## PHPCS

Again under the main preferences window, search for Code Sniffer. Two sections will be available:

### Languages and Frameworks

Here is where you setup PHPStorm to point to the right command line script for code sniffer. On Configuration, click the ```...``` to bring up the finder window. Select ```openeyes/bin/phpcs```

### Editor -> Inspections

You need to select the coding standard which is included with OpenEyes. On the coding standard dropdown select "Custom". Then click the ```...``` to browse to ```openeyes/build```
