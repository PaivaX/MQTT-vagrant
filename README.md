 
# Projeto MQTT Broker 
Criação de um ambiente de desenvolvimento, utilizando o Vagrant em conjunto com o VirtualBox, e utilizando o equipamento IOT Raspberry pico W.
Foram definidos alguns requisitos, e implementados no projeto.



# Índice  
1. [Introdução](#projeto-mqtt-broker)  
2. [Tech Stack](#tech-stack)    
3. [Características](#Características) 
4. [O que aprendi?](#o-que-aprendi)
5. [Iniciar o projeto](#iniciar-o-projeto)
6. [Variáveis](#variáveis)
7. [Comandos úteis](#comandos-úteis)
7. [Relatório](#relatório)
8. [Bibliografia](#Bibliografia)
9. [Licença](#Licença)


## Screenshots  

![App Screenshot](https://github.com/PaivaX/MQTT-vagrant/blob/main/share/logo.png?raw=true)

## Tech Stack  

**Client:** ubuntu, paho MQTT  

**Server:** ubuntu, MQTT Mosquitto

**Raspberry Pico:** MycroPython

## Características  

VM´s:
- Instalação e configuração automática das VM   
- Instalação e configuração do broker Mosquitto  
- Instalação do cliente paho MQTT  

Raspberry Pico w:
- Ligar ao wireless com indicação Led de sucesso e mensagem
- Ligação ao broker
- Envio da temperatura
- Receção de instrução para Ligar/desligar Led 

## O que aprendi?  

A configurar o Vagrantfile, para duas máquinas virtuais, com especificações distintas.

A criar scripts SHELL, para instalar módulos e configurar os mesmos.

A configurar o raspberry Pico W, para ligar ao Wireless, Broker, e publicação e subscrição de tópicos MQTT


## Iniciar o projeto 

Clonar o projeto  

~~~bash  
  git clone https://github.com/PaivaX/MQTT-vagrant.git
~~~

Ir para o diretório do projeto  

~~~bash  
  cd vagrant-mqtt
~~~

Iniciar as VM  

~~~bash  
vagrant up
~~~

## Variáveis  

Definir o user e password, no ficheiro "install_mosquitto.sh":  
`user`

`password`  

Para alterar o tópico, deve ser alterado no ficheiro mqtt_sub.py

`topic` 


## Comandos úteis

Entrar no SSH da VM.
~~~bash 
vagrant ssh <nome_vm>
~~~

Iniciar VM

~~~bash
vagrant up <nome_vm>
~~~

Desligar VM

~~~bash
vagrant halt
~~~~

Destruir VM. O código-fonte e o conteúdo do diretório de dados permanecerão inalterados. 
Somente a instância da máquina VirtualBox será destruída. Pode-se construir a VM com o comando 'vagrant up'.
Este comando é útil se você deseja economizar espaço em disco.
#### Aviso: este comando destruirá os bancos de dados do seu site.
Backup da BD: sql-dump > db.sql 
~~~bash 
vagrant destroy
~~~

Reconfigurar VM depois de alterações ao código fonte.
~~~bash
vagrant provision
~~~

Recarregar VM. Útil quando se altera as propriedades de rede.
~~~bash$
vagrant reload
~~~

## Relatório  

Escrever relatório

## Bibliografia  

- [Peppe8o](https://peppe8o.com/mqtt-and-raspberry-pi-pico-w-start-with-mosquitto-micropython/)
- [Steve´s Internet Guide](http://www.steves-internet-guide.com/mqtt/)
- [Tomshardware](https://www.tomshardware.com/how-to/connect-raspberry-pi-pico-w-to-the-internet)


## Licença  

Este é um software gratuito e sem custo distribuído no domínio público.

Qualquer pessoa é livre para copiar, modificar, publicar, usar, compilar, vender ou
distribuir este software, seja em forma de código-fonte ou compilado, para qualquer finalidade, comercial ou não comercial.

Para mais informações, <https://unlicense.org>