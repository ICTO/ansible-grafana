Grafana
=========

Ansible role that handles the installation of grafana to a specified directory.

The installation and configuration of the webserver is not handled in this role.

Requirements
------------

/

Role Variables
--------------

Example should be self-explanatory :


```
grafana:
  home: /home/grafana
  install_dir: grafana
  version: 1.8.1
  webroot: /var/www/grafana
  datasources:
    - name: graphite
      type: graphite
      url: localhost
    - name: elasticsearch
      type: elasticsearch
      url: localhost
      index: grafana-dash
  admin:
    password: 'topsecret'

```
