Данный скрипт делал для себя с целью быстрой развертки основных компонентов K8S на несколько нод и дальнейшей развертке кубернетиса.

В установке присутсвует Zabbix-agent для мониторнга состояния узлов, он никак не преднастроен в дальнейшем планирую исправить это и дать возможность указывать сервер Zabbix в конфиг файл агента для безопастности. 

Вы также можете закоментить установку Zabbix агента в файле prepare-k8s-lab.yml

Для запуска скрипта отредактируйте файл "inventory" по примерам в данном файле также не забудьте добавить ssh ключи на удаленные сервера

Затем перейдите в дерикторию k8s-ansible-playbook/ansible-playbooks и запустите команду "ansible-playbook prepare-k8s-lab.yml -i inventory"

Данный скрипт работает на версии ansible 2.10.8
