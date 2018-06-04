# Установка Pritunl VPN server на ubuntu 16.04 c использованием Ansible=>2.5

## Установка
Для установки необходимо: 
- создать файл inventory в директории `environments/stage/` на осонове файла inventory.example
- последовательно выполнить команды, находясь в корне рипозитория: 
  - `ansible-galaxy install -r environments/stage/requirements.yml`
  - `ansible-playbook -i environments/stage/inventory playbooks/pritunl_start.yml`
- зайти через браузер на ip хоста и выполнить дальнейшую настройку Pritunl.
