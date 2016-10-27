# Ansible Role: Sublime Text (Drupal Configurator)

[![Build Status](https://travis-ci.org/fubarhouse/fubarhouse.sublime-drupal.svg?branch=master)](https://travis-ci.org/fubarhouse/fubarhouse.sublime-drupal)

Configures Sublime using the [recommended Drupal standard](https://www.drupal.org/docs/develop/development-tools/configuring-sublime-text) on macOS.

## Requirements

 - Sublime Text

## Role Variables

### URL of packagemanager settings file:
`sublime_packageman_file: https://packagecontrol.io/Package%20Control.sublime-package`

### Array of Sublime packages to install

See defaults/main.yml for all entries, the following is an example.

````
- STPackages:
- name: DrupalSublimeConfig;
  repository: https://github.com/enzolutions/drupal-sublime-config.git
````

## Dependencies

None.

## Example Playbook

    - hosts: localhost
      roles:
        - fubarhouse.sublime-drupal

## License

MIT / BSD

## Author Information

This role was created in 2016 by [Karl Hepworth](twitter.com/fubarhouse).
