# ansible-role-php

[![Build Status](https://travis-ci.org/kosssi/ansible-role-php.svg?branch=master)](https://travis-ci.org/kosssi/ansible-role-php)

Install and configure PHP

## Role Defaults Variables

    php_repository: ppa:ondrej/php5

    php_install:
      - php5

    php_configure:
      - file: /etc/php5/cli/php.ini
        values:
          - { section: date, key: date.timezone, value: 'Europe/Paris' }

## Example Playbook

    roles:
      - { role: kosssi.php, tags: php }

## License

Licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
