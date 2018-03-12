# CQPweb CSS Styles
This is a simple set of styles for CQPweb, briefly tested on v3.2.31. It uses global variables to define a color scheme and is thus easily customizable. Further customization and refinement, e.g. of aligning table columns based on their content, would require changes to the main code and is currently not planned.

twi_corpora.css contains main CSS definitions for corpus view. 
twi_scheme_COLOR.css provide different color schemes for corpora and import definitions, using twi_corpora.css as basis.
twi_main.css is a version of twi_corpora.css adjusted for the CQPweb main page.

## Installation
Download the files and move to you the cqpweb/css directory on your web server.

## Use corpus schemes
Go to "Corpus settings" and change Stylesheet address to the desired scheme (e.g. ../css/twi_scheme_red.css).

## Use main page scheme
Add or modify the following line in cqpweb/lib/config.inc.php:
$css_path_for_homepage = 'css/twi_main.css';

## Customize color schemes 
To add a new corpus color scheme copy one of the twi_scheme_COLOR.css files and adjust the color definition as desired.
To change the main page color scheme, adjust color values in twi_main.css.

