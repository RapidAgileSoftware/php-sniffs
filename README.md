php-codestyles
=======

Rapid Agile Software default code styles to be used with Squizlabs' codesniffer and PHPCSFixer.

## Install

1) Create a file `easy-coding-standard.neon` in the root path of project with at least below contents:
```yml
includes:
  - vendor/ras/sniffs/easy-coding-standard.neon

```

2) Run `composer require-dev ras/sniffs`

43 Add a linting command to `composer.json`

```
  "scripts": {
    "lint": "ecs check src cron tests --clear-cache",
    "lint:fix": "ecs check src cron tests --clear-cache --fix"
  }
```
