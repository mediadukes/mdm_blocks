# Custom Drupal 8 module for pre-configured blocks

This module installs Drupal core block and adds some useful configurion:

- A basic block type to add simple textual blocks
- If the [geolocation](https://www.drupal.org/project/geolocation) module and it's google map submodule are enabled it will add a block type to create google maps.
- When the [mdm_paragraphs](https://github.com/mediadukes/mdm_paragraphs) module is enabled it will add a block paragraph type using modules like [inline_entity_form](https://www.drupal.org/project/inline_entity_form) and [entity_browser](https://www.drupal.org/project/entity_browser) for an easy UX.

## Usage

Just install as any other drupal module using `composer require`.

```
composer require mediadukes/mdm_blocks:^1.0
```

If it's not already present in your repositories array you'll need to define inside your root `composer.json` where mediadukes packages can be found.

```
"repositories": [
  {
    "type": "composer",
    "url": "https://packages.mediadukes.be"
  }
]
```

Or you can use the [mediadukes drupal-project template](https://github.com/mediadukes/drupal-project) where the repository is already in combination with the custom [Amatus profile](https://github.com/mediadukes/mdp_amatus).
