# Ansible Infrastructure Automation 
## Provisionamento e Hardening de Servidores Linux

Este projeto tem como objetivo demonstrar o uso do Ansible para automação de **infraestrutura**, realizando o provisionamento completo de servidores Linux de forma padronizada e segura, além de conter uma documentação explicativa e didática sobre as estruturas.

A solução automatiza tarefas comuns do dia a dia de um Analista de **TI / DevOps**, como configuração inicial do sistema, criação de usuários, instalação de serviços e deploy de aplicações, reduzindo erros manuais e garantindo consistência entre os servidores.

Ambiente utilizado:
- Uma máquina virtual com Ubuntu Server 25.10, como **control node**.
- Três máquinas virtuais com Ubuntu Server 24, como **managed nodes**.

### Funcionalidades automatizadas
- Atualização do sistema operacional e instalação de pacotes essenciais
- Criação e gerenciamento de usuários com autenticação via chave SSH
- Configuração de acesso sudo e políticas básicas de segurança

### Tecnologias utilizadas
- **Ansible**
- Linux (Ubuntu Server)
- SSH
- Docker

### Estrutura do projeto

ansible-infra-automation/  
├── Docs  
│   ├── [Add_Control_Node.md](./Docs/Add_Control_Node.md)  
│   └── [Ansible_Plugins.md](./Docs/Ansible_Plugins.md)  
├── inventories/  
│   └── [hosts.ini](./inventories/hosts.ini)  
├── playbooks/  
│   ├── [site.yaml](./playbooks/site.yaml)  
│   ├── [users.yaml](./playbooks/users.yaml)  
│   ├── [docker.yaml](./playbooks/docker.yaml)  
│   └── [webserver.yaml](./playbooks/webserver.yaml)  
├── roles/  
│   ├── [users/](./roles/users/)  
│   ├── [nginx/](./roles/nginx/)  
│   └── [docker/](./roles/docker/)  
├── [ansible.cfg](./ansible.cfg)  
└── [README.md](./README.md)  