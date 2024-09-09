# Preparação de ambiente
### Vamos prepara o ambiente para desenvolvimento de aplicações

#### Nesta preparação iremos instalar e configurar os seguintes recursos:
 - Máquina virtual (VirtualBox)
 - Distribuição Linux (Ubuntu Server)
 - Nasm
 - Compilador de linguagem C
 - Configurar o IP e a porta de comunicação entre a máquina real e a virtual
 - Configurar o acesso via SSH entre o VSCode e o servidor Linux
 - Configurar as extensões: Material Icon, Nasm, SSH e linguagem C/C++

 #### Máquina virtual (VirtualBox)

 !["Logo VirtualBox"](virtualbox.png)

 Máquina virtual é uma ferramenta que permite a criação de novos computadores e a instalação de sistemas operacionais, para estudo ou trabalho.

 Para nosso estudo iremos usar o VirtualBox da Oracle.
 Para fazer o download no link a seguir:

 <a href="https://www.virtualbox.org/wiki/Downloads" target="_blank"> VirtualBox </a>

 ##### Criando a máquina virtual para o nosso estudo

 - Configuração:
    > - Nome da máquina: Servidor
    > - Memória: 4GB(4096)
    > - Processador: 2
    > - Disco: 100GB
    > - IP e porta do Host: 127.0.0.1 e 22
    > - IP e porta do convidado: 10.0.2.15 e 22

- Tela inicial de configuração

<img src=vmconfig01.png width=500 height=400>

- Tela de configuração do Hardware

<img src=vmconfig02.png width=500 height=400>

- Tela de configuração do Disco

<img src=vmconfig03.png width=500 height=300>

- Tela de sumário

<img src=vmconfig04.png width=500 height=300>

- Tela de configuração de rede

<img src=vmconfig05.png width=500 height=350>

- Tela de configuração de portas e IPs

<img src=vmconfig06.png width=500 height=250>

#### Distribuição Ubuntu Server

<img src=ubuntu_logo_orange.png width=300 height=135>

Para o nosso estudo iremos utilizar uma distribuição Linux para servidores chamada Ubuntu. Acompanhe o processo de instalação:

Faça o download aqui:

<a href="https://ubuntu.com/download/server" target="_blank"> Ubuntu Server </a>

- Acompanhe a instalação:

- Tela de início de instalação

<img src=ubuntuinstal01.png>

- Tela de seleção de idioma

<img src=ubuntuinstal02.png>

- Tela de seleção de teclado

<img src=ubuntuinstal03.png>

- Tela de tipo de instalação

<img src=ubuntuinstal04.png>

- Tela de configuração do proxy

<img src=ubuntuinstal05.png>

- Tela de pacotes de atualização

<img src=ubuntuinstal06.png>

- Tela de configuração do disco 

<img src=ubuntuinstal07.png>

- Tela de configuração do usuário

<img src=ubuntuinstal08.png>

- Tela de configuração do SSH

<img src=ubuntuinstal09.png>

- Tela do fim da instalação

<img src=ubuntuinstal10.png>

#### Atualização do Sistema 

Para a correta utilização do servidor Ubuntu que acabamos de instalar, será necessário realizar a atualização do sistema.

- Execute o comando abaixo:

```
sudo apt update -y && sudo apt upgrade -y
```

- Reinicie o seu servidor usando o comando abaixo:

```
reboot 
```

#### Instalação do Compilador NASM

O compilador do NASM é uma ferramenta que nos permite programar em Assembly. Assim é possivel criar programas que manipulam dados que estão nos registradores do processador.

- Para instalar o NASM no Ubuntu, usamos o comando:

```
sudo apt install nasm -y
```

#### Instalação do compilador da Linguagem C

Em Linux, o compilador da Linguagem C é o GCC. Ele é uma ferramenta importante para o desenvolvimento de programas em C.

Pra instaladar use o comando:
```
sudo apt install gcc -y
```

#### Conexão Servidor e VSCode via SSH

Precisamos instalar uma extensão no VSCode para acessar o nosso servidor de forma remota.

!["Extensão SSH"](extensaossh.png)

Configuração do acesso remoto.

!["Configuração"](configurarextensao.png)
