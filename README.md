ansible-role-zookeeper
=========

Role de instalação do zookeeper


Role Variáveis
--------------

Essa role possui algumas variáveis padrões que podem ser alterados de acordo com o seu ambiente.
```yml
path_zoo: /etc/zookeeper 
user_zoo: zoouser
version_zoo: 3.4.14
init_limit_zoo: 5
sync_limit_zoo: 2
client_port_zoo: 2181
data_dir_zoo: /var/lib/zookeeper
log_dir_zoo: /var/log/zookeeper
```

Dependencias
------------

Para a instalação do zookeeper, é preciso ter o java instalado. Por conta disso essa role possui uma dependência de uma outra role que é a instalação do kafka, antes de executar essa role você deve baixar a role que no qual esta depende com o seguinte comando: 
```shell
# ansible-galaxy install -r requeriments.yml
```

Examplo Playbook
----------------

Abaixo um exemplo do arquvivo de playbook para a instalação:

    - hosts: servers
      roles:
         - zookeeper

License
-------

BSD

Informação do Autor
------------------
Alvaro Bacelar - Especialista em Infraestrutura, entusiasta DevOps e Infra As Code
