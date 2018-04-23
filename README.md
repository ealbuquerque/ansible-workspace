# Instalação de ambiente de desenvolvimento padrão ZarthJr de qualidade :thumbsup: :poop:

Instalação do ambiente de desenvolvimento padrão.

Suporte apenas para **Ubuntu**

## Passos de instalação

* Instalar o Ansible:

```bash
$ sudo apt-get update
$ sudo apt-get install software-properties-common
$ sudo apt-add-repository ppa:ansible/ansible
$ sudo apt-get update
$ sudo apt-get install ansible
```

* Baixar este projeto
* Alterar o host do playbook.yml para localhost (instalação local) ou para O VagrantFile, caso queira testar.
* Alterar a variável de usuário em ./group_vars/all.yml para o usário criado na instalação do S.O.
* Para rodar:
  * Ansible-playbook -vv  playbook.yml --extra-vars 'ansible_become_pass=zzzz'

## Próximos Passos

* Instalação:
  * Android Studio
  * Nvidia Drivers
  * Steam
  * DataGrip
  * GoLand (https://gist.github.com/szarthjr/88ceae7b0aedc38410d4de65764c1fae)
  * IntelliJ
  * Rider
  * Turtl
* Disable do auto update
* Replicar configurações dos softwares mais usados
* Instalação das extensões do gnome e suas respectivas configurações
  * User Themes
  * Top Icons Plus
  * No Title Bar
* Criação de handler para apt
* Fontes do sistema
* Remoção do problema com o repo security 
* Instalar os extras do virtualbox
* Fazer uma versão para o windows
