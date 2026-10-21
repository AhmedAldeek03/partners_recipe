# Partners

Adds a **Partner** content type (`partner`) for partner, client and sponsor logos.

## What it adds

- `field_media`: logo (required)
- `field_link`: website
- `field_term`: type (Partner types vocabulary)

## Blocks and pages

- **Partners: Logos** block: every logo, linked to the partner website, without titles.

## Conventions

- Fields are named after their field type (`field_text`, `field_media`, `field_term`, …), never after
  their purpose or content type, so recipes share them. Shared fields are identical across all our
  recipes, so they can be applied in any order on the same site.
- Edit forms are grouped into **Basic information** and **Media** sections.
- View modes: **Default** (full page) and **Card** (listings).
- The **Content editor** role gets create, edit, delete and revision permissions.

## Requirements

- Drupal 11

## Installation

```bash
composer config repositories.partners_recipe '{"type": "vcs", "url": "https://github.com/AhmedAldeek03/partners_recipe", "no-api": true}'
composer require drupal/partners_recipe:1.0.x-dev@dev
drush recipe ../recipes/partners_recipe
drush cache:rebuild
```

With DDEV, put `ddev` before each command.
