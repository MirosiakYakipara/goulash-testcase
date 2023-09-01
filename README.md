# goulash-testcase

Для генерации inventory файла необходимо выполнить команду: ansible-playbook --tags create_inv playbook.yml

Для создания mysql необходимо выполнить команду: ansible-playbook -i inventory --tags install_mysql playbook.yml

Для добавления базы необходимо выполнить команду: ansible-playbook -i inventory -e "db_name=dev db_user=dev db_user_password=passs" -t install_mysql playbook.yml
