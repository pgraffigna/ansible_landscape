# ansible_landscape

Ansible Playbook para desplegar un Servidor Landscape + clientes.

Testeado con Vagrant + Virtualbox + Ubuntu18.04

---
### roles

- server
- client

### Instalar Servidor
ansible-playbook server_setup.yml --limit IP/HOST

### Instalar Cliente
ansible-playbook client_setup.yml --limit IP/HOST

---
### Notas
- la instalación del server se toma su tiempo
- cuando ejecutamos la receta para el cliente tenemos que aprobar la petición desde el dashboard de landscape sino ansible tira un timeout ya que se queda esperando la aprobación.



