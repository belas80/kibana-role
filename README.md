Kibana role
=========

Роль для установки kibana на хостах с ОС: Debian, Ubuntu, CentOS, RHEL.

Requirements
------------

Поддерживаются только ОС семейств debian и EL.  

Role Variables
--------------

* kibana_version (default: "7.14.0") - Параметр, который определяет какой версии kibana будет установлена
* Имя хоста Elasticsearch в шаблоне конфига кибаны [templates/kibana.yml.j2](templates/kibana.yml.j2), считывается из hostvars (default: 'el-instance').

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: kibana-role }

License
-------

MIT

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
