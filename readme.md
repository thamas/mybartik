# MyBartik :)

Fork of Drupal 8's Bartik theme for my theming presentations (about Twig).  
(Do Not use Bartik as a base theme in real projects, 'cause updates may break
your theme!')
It looks broken because markup was changed but CSS styling was not created for
the new classes! :)

- https://www.drupal.hu/konferencia/2016/program#smink
- http://2016.drupalaton.hu/schedule#speaker-151

Files to check:
- node.html.twig
  - added new variable: bundle
  - use BEM style class naming where block is the content type
  - added embedded twig block, to split up template to smaller parts
- node--article.html.twig
  - new file, extends node.html.twig
- node--article--teaser.html
  - new file, extends node--article.html.twig
  - example usage of "parent"
  - added custom read more link using path function
- page.html.twig
  - Current date using format_date
  - Kint
  - (try to) print content of different node fields
  - Copyright message using date() filter
- menu.html.twig
  - new file
  - added custom css classes (article link below)
- mybartik.theme
  - preprocess to have "bundle" variable in field.html.twig
  - template suggestions sample for custom block types
- field.html.twig
  - new file to add "BEM Element" style class to fields
- field--node--field-tags.html.twig
  - added first / last classes and tag count using Twig's loop variable

Related info:
- [Twig Documentation](http://twig.sensiolabs.org/documentation)
- [Set Twig Debug](https://www.drupal.org/node/2259531)
- [Drupal 8 Twig: add custom CSS classes to menus (based on menu name)](https://medium.com/integral-vision/drupal-8-twig-add-custom-css-classes-to-menus-based-on-menu-name-35b50142521a#.2lg9fvoeq)
- [Applying BEM inspired classes to your Drupal 8 theme](https://thejibe.com/articles/applying-bem-inspired-classes-to-your-drupal-8-theme)
