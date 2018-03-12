# CQPweb CSS Styles
This is a simple set of styles for CQPweb, briefly tested on v3.2.31 and with current versions of Chrome, Safari and Firefox. It has templates for blue, green, yellow and red. Since the CSS files use global variables to define colors, it is very easily customizable. If you find objectively ugly views or have suggestions for improvements, please create an issues. Note that further refinements, e.g. on result table display and text alignment of column content, currently cannot be done at the CSS level, but would require changes to the main code.

*twi_corpora.css* contains main CSS definitions for corpus view. 
*twi_scheme_COLOR.css* provide different color schemes for corpora and import definitions, using twi_corpora.css as basis.
*twi_main.css* is a version of twi_corpora.css adjusted for the CQPweb main page.

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



– 12.3.2018, Thilo Wiertz
