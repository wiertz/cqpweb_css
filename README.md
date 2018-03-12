# CQPweb CSS Styles
This is a simple set of styles for CQPweb, briefly tested on v3.2.31 and with current versions of Chrome, Safari and Firefox. It has templates for blue, green, yellow and red. Since the CSS files use global variables to define colors, it is very easily customizable. If you find objectively ugly views or have suggestions for improvements, please create an issues. Note that further refinements, e.g. on result table display and text alignment of column content, currently cannot be done at the CSS level, but would require changes to the main code.

- *style-corpus.css* contains main CSS definitions for corpus views. 
- *corpus-COLOR.css* provide different color schemes for corpora. Requires and imports style-corpus.css.
- *style-main.css* is a version of style-corpus.css, but adjusted for the CQPweb main page.

## Installation
Download .css files and copy to the css subdirectory of cqpweb on your web server (e.g. /var/www/cqpweb/css).

## Use corpus schemes
Go to "Corpus settings" and change Stylesheet address to the desired scheme (e.g. ../css/corpus-red.css).

## Use main page scheme
Add or modify the following line in /lib/config.inc.php:
$css_path_for_homepage = 'css/style-main.css';

## Customize color schemes 
To add a new corpus color scheme copy one of the corpus-COLOR.css files and adjust the color definition as desired.
To change the main page color scheme, adjust color values in style-main.css.

## Screenshots

#### Main corpus view:
![Corpus](/screenshots/blue_corpus.png)

#### Query results (keyword in context):
![KWIC](/screenshots/blue_kwic.png)

#### Collocation table:
![Collocations](/screenshots/blue_collocations.png)

#### Yellow scheme example:
![Collocations](/screenshots/yellow_keywords.png)

– 12.3.2018, Thilo Wiertz
