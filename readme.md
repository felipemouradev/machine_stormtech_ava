***Instalação Maquina Virtual***

Levando em consideração a avaliação deve funcionar em uma instalação limpa do ubuntu 16.04

Os passos para instalação do Virtualbox podem ser encontrados também no site:
[https://www.virtualbox.org/wiki/Linux_Downloads](https://www.virtualbox.org/wiki/Linux_Downloads)

***Instalando o Virtualbox***


Instalando o Virtualbox, adione o repositorio do virtualbox na sua lista de repositorios executando o comando a seguir:

```
$ sudo sh -c  'echo "deb http://download.virtualbox.org/virtualbox/debian xenial contrib" >> /etc/apt/sources.list'
```
Registrando

```
 $ wget -q https://www.virtualbox.org/download/oracle_vbox_2016.asc -O- | sudo apt-key add -
 $ wget -q https://www.virtualbox.org/download/oracle_vbox.asc -O- | sudo apt-key add -

```

Atualizando pacotes e instalando o Virtualbox:

```
$ sudo apt-get update && sudo apt-get install virtualbox-5.1
```

***Instalando o Vagrant***

Nesse site você pode fazer o download do vagrant [https://www.vagrantup.com/downloads.html](https://www.vagrantup.com/downloads.html), baixe de versão para debian e de acordo com sua arquitetura de sistema operacional (32 bits ou 64bits)

logo apos no diretorio onde você fez download, execute:

```
$ dpkg -i nome_do_pacote_vagrant_que_voce_baixo.deb
```

Também é necessario a instalação do git:

```
$ sudo apt-get install git
```

Clone o esse repositorio:

```
$ git clone https://github.com/felipemouradev/machine_stormtech_ava
```

Em seguida:

```
$ cd machine_stormtech_ava && vagrant up
```


Isso irá instalar todas as depencias da vm e subir uma instância da mesma.

Após isso, altere o /etc/hosts, acrescente:

```
192.168.56.101  wwww.books.dev
```
Salve...

agora o serviço estára disponivel em [www.books.dev]( www.books.dev)

