# openvpn client install ansible role playbook

Group variables:

* ansible_ssh_private_key_file

Файл содержащий ключ для ssh авторизации на ec2.
default: /home/ubuntu/gtarada.pem

* ansible_ssh_user

Имя пользователя для автторизации на ec2.
default: ubuntu

Openvpn role variables:

* openvpn_ca_file

Содержимое файла ca с сертификатом CA.

* openvpn_cert_file

Содержимое файла cert с сертификатом клиента.

* openvpn_key_file

Соедржимое файла key с ключом клиента.

* openvpn_package_version

Версия apt пакета openvpn.
default: 2.3.10-1ubuntu2.1.
Глобальна для роли

* openvpn_port_openvpn_client_conf

Порт на стороне openvpn сервера для подключения.
default: 2195

* openvpn_proto_openvpn_client_conf

IP протокол используемый для openvpn подключения.
default: udp.
Глобальна для роли

* openvpn_server_openvpn_client_conf

IPv4 адрес openvpn сервера.
default: 8.8.8.8

* openvpn_tls_auth_file

Содержимое файла tls-auth с ключом для TLS-AUTH.
A