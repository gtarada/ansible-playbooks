# openvpn client install ansible role playbook

Group variables:

* ansible_ssh_private_key_file
Файл содержащий ключ для ssh авторизации на ec2
default: /home/ubuntu/gtarada.pem

* ansible_ssh_user: ubuntu
Имя пользователя для автторизации на ec2
default: ubuntu

Openvpn role variables:

* openvpn_package_version
Версия apt пакета openvpn
default: 2.3.10
Глобальна для роли

* openvpn_port_openvpn_client_conf
Порт на стороне openvpn сервера для подключения
default: 2195

* openvpn_proto_openvpn_client_conf
IP протокол используемый для openvpn подключения
default: udp
Глобальна для роли

* openvpn_server_openvpn_client_conf
IPv4 адрес openvpn сервера
default: 8.8.8.8
