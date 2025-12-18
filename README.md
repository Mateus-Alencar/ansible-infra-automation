# Ansible Infrastructure Automation 
## Provisionamento e Hardening de Servidores Linux

Este projeto tem como objetivo demonstrar o uso do Ansible para automação de **infraestrutura**, realizando o provisionamento completo de servidores Linux de forma padronizada e segura.

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
├── inventories/  
│   └── hosts.ini  
├── playbooks/  
│   ├── site.yaml  
│   ├── users.yaml  
│   ├── docker.yaml  
│   └── webserver.yaml  
├── roles/  
│   ├── users/  
│   ├── nginx/  
│   └── docker/  
├── ansible.cfg  
└──  README.md  
