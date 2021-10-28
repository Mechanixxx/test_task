#### Задание-обучение на практику с Ansible

Виртуалки подняты на Virtualbox, ОС - Ubuntu 18.04, RAM 1024Mb network - Bridge

Проект построен по типовой схеме, переменная переопределяется.

Роль присутствует, шаблон работает.

1. Настраиваем доступ к машинкам по ssh-ключам
2. Запускаем по очереди scenario_one, scenario_two

```
ansible-playbook -i inventoies/prod/hosts inventories/prod/scenario_one.yml
ansible-playbook -i inventoies/prod/hosts inventories/prod/scenario_two.yml
```
