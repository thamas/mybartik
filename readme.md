# MyBartik :)

Fork of Drupal 8's Bartik theme for my theming presentations (about Twig).
(Do Not use Bartik as a base theme in real projects, 'cause updates may break
your theme!)

Warning: It looks broken because markup was changed but CSS styling was not
written for the new classes! :)

## Files to check:
- block.html.twig
  - add bundle (type) class to blocks
- field.html.twig
  - new file to add "BEM Element" style class to fields
- field--node--field-tags.html.twig
  - added first / last classes and tag count using Twig's loop variable
- menu.html.twig
  - new file
  - added custom css classes (article link below)
- mybartik.theme
  - preprocess to have "bundle" variable in field.html.twig
  - template suggestions sample for custom block types
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
  - Copyright message using date() filter
  - Current date using format_date
  - Node created and updated date
  - Kint
  - (try to) print content of different node fields

## Things to read:
- [Twig Documentation](http://twig.sensiolabs.org/documentation)
- [Set Twig Debug](https://www.drupal.org/node/2259531)
- [Drupal 8 Twig: add custom CSS classes to menus (based on menu name)](https://medium.com/integral-vision/drupal-8-twig-add-custom-css-classes-to-menus-based-on-menu-name-35b50142521a#.2lg9fvoeq)
- [Translatable, custom dates in Twig templates of Drupal 8](https://medium.com/p/140c91330c2b)
- [Applying BEM inspired classes to your Drupal 8 theme](https://thejibe.com/articles/applying-bem-inspired-classes-to-your-drupal-8-theme)
- [Things I Learned from the DrupalTwig Slack: Volume 1](http://www.annertech.com/blog/things-learned-drupal-twig-slack-volume-1)
- [Things I Learned from the DrupalTwig Slack: Volume 2](http://www.annertech.com/blog/things-learned-drupal-twig-slack-volume-2)
- [Pistachio: "…to serve as an example of all the features a theme can have"](https://www.drupal.org/project/pistachio)
- [Top Thirteen Drupal Twig Helper Modules](https://www.xenomedia.com/blog/top-thirteen-drupal-twig-helper-modules)
- [Introducing the UI Patterns module: use atomic UI components everywhere in Drupal 8](http://nuvole.org/blog/2017/jan/23/ui-patterns-module-re-use-ui-components-everywhere-in-drupal-8)

## Theming related modules:
- https://www.drupal.org/project/components – Registers “component libraries” defined by your theme or module as Twig namespaces.
- https://www.drupal.org/project/twig_field_value
- https://www.drupal.org/project/themable_forms
- https://www.drupal.org/sandbox/mikeker/2612132 (Twig Globals)
- https://www.drupal.org/project/ui_patterns – "Define and expose self-contained UI patterns as Drupal plugins and use them seamlessly in your Paragraphs, Panels, Field Groups or Display Suite view modes.""
