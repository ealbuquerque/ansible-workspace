# Instalação de ambiente de desenvolvimento

Instalação do ambiente de desenvolvimento padrão.

Suporte apenas para **Ubuntu**

## Passos de instalação

1. Instalar o Ansible:

```bash
sudo apt-get update && \
sudo apt-get install software-properties-common && \
sudo apt-add-repository ppa:ansible/ansible && \
sudo apt-get update && \
sudo apt-get install ansible
```

2. Clonar este projeto

```bash
git clone https://github.com/ealbuquerque/ansible-workspace.git
```

3. Alterar o host do playbook.yml para localhost (instalação local) ou para O VagrantFile, caso queira testar.

4. Alterar a variável de usuário em ./group_vars/all.yml para o usário criado na instalação do S.O.

5. Para rodar:

```bash
ansible-playbook -vv  playbook.yml --extra-vars 'ansible_become_pass=YOUR_PASSWORD'
```

## Próximos Passos

* Instalação:
  * Android Studio
  * Nvidia Drivers
  * Steam
  * DataGrip
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
