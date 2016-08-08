# MyBartik :)

Fork of Drupal 8's Bartik theme for my theming presentations.  
(Do Not use Bartik as a base theme in real projects, 'cause updates may break
your theme!')

- https://www.drupal.hu/konferencia/2016/program#smink
- http://2016.drupalaton.hu/schedule#speaker-151

Files to check:
- node.html.twig
  - added new variable: bundle
  - added embedded twig block, to split up template to smaller parts
- node--article.html.twig
  - new file, extends node.html.twig
- node--article--teaser.html
  - new file, extends node--article.html.twig
  - example usage of "parent"
- page.html.twig
  - Kint
  - (try to) print content of different node fields
- menu.html.twig
  - new file
  - added custom css classes (article link below)

Related info:
- [Twig Documentation](http://twig.sensiolabs.org/documentation)
- [Set Twig Debug](https://www.drupal.org/node/2259531)
- [Drupal 8 Twig: add custom CSS classes to menus (based on menu name)](https://medium.com/integral-vision/drupal-8-twig-add-custom-css-classes-to-menus-based-on-menu-name-35b50142521a#.2lg9fvoeq)
