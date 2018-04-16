# Instalação de ambiente de desenvolvimento padrão ZarthJr de qualidade :thumbsup: :poop:

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
  * DataGrip
  * GoLand
  * IntelliJ
  * Rider
  * Turtl
* Configuração dos paths do Go
* Replicar configurações dos softwares mais usados
* Instalação das extensões do gnome e suas respectivas configurações
  * User Themes
  * Top Icons Plus
  * No Title Bar
* Fazer uma versão para o windows