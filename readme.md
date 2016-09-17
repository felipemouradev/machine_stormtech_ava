***Instalação Maquina Virtual***

É necessario a instalação do Virtual box, Vagrant que podem ser encontradas nos links respectivos

https://www.virtualbox.org/wiki/Linux_Downloads

https://www.vagrantup.com/downloads.html

Também é necessario a instalação do git:

```
$ sudo apt-get install git
```

Clone o projeto:

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

