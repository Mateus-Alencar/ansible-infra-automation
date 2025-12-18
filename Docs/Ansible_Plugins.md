## Ansible Plugins
No Ansible, o arquivo **`ansible.cfg`** permite configurar plugins para estender ou alterar o comportamento da ferramenta. Esses plugins são habilitados e configurados por categoria, apontando caminhos, prioridades ou opções padrão.

Plugins disponíveis no **`ansible.cfg`**:
```
- base       # define funcionalidades fundamentais para outros plugins Ansible.
- become     # escalonar privilégios, permite executar comandos com permissões elevadas (sudo, su).
- cache      # gerencia o cache de fatos (facts) coletados para acelerar execuções futuras.
- callback   # controla a saída do Ansible, permite customizar como os resultados são exibidos.
- cliconf    # configuração de dispositivos de rede via CLI (interface de linha de comando).
- connection # gerencia o método de conexão com os hosts remotos (SSH, local, paramiko, etc).
- httpapi    # permite comunicação com dispositivos via APIs HTTP/REST.
- inventory  # obtém e gerencia o inventário de hosts, podendo ser estático ou dinâmico.
- lookup     # busca dados de diferentes fontes (arquivos, variáveis, bases externas).
- netconf    # comunicação com dispositivos de rede via protocolo NETCONF.
- shell      # executa comandos shell nos hosts remotos como parte da conexão.
- vars       # gerencia variáveis dentro do Ansible, permitindo manipulação e definição.
```