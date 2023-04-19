 
# Projeto MQTT Broker 
Criação de um ambiente de desenvolvimento, utilizando o Vagrant em conjunto com o VirtualBox, e utilizando o equipamento IOT Raspberry pico W.
Foram definidos alguns requisitos, e implementados no projeto.



# Índice  
1. [Introdução](#projeto-mqtt-broker)  
2. [Tech Stack](#tech-stack)    
3. [Características](#Características) 
4. [O que aprendi?](#)
5. [Iniciar o projeto](#)
6. [Variáveis](#)
7. [Relatório](#)
8. [Licença] (#)


## Screenshots  

![App Screenshot](https://github.com/PaivaX/MQTT-vagrant/blob/main/share/logo.png?raw=true)

## Tech Stack  

**Client:** ubuntu, paho MQTT  

**Server:** ubuntu, MQTT Mosquitto

**Raspberry Pico:** MycroPython

## Características  

- Light/dark mode toggle  
- Live previews  
- Fullscreen mode  
- Cross platform 

## O que aprendi?  

A configurar o Vagrantfile, para duas máquinas virtuais, com especificações distintas.

A criar scripts SHELL, para instalar módulos e configurar os mesmos.

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

Start the server  

~~~bash  
npm run start
~~~

## Variáveis  

To run this project, you will need to add the following environment variables to your .env file  
`API_KEY`  

`ANOTHER_API_KEY` 

## Bibliografia  

- [Awesome Readme Templates](https://awesomeopensource.com/project/elangosundar/awesome-README-templates)
- [Awesome README](https://github.com/matiassingers/awesome-readme)
- [How to write a Good readme](https://bulldogjob.com/news/449-how-to-write-a-good-readme-for-your-github-project)

## Relatório  

Escrever relatório

## Licença  

Este é um software gratuito e sem custo distribuído no domínio público.

Qualquer pessoa é livre para copiar, modificar, publicar, usar, compilar, vender ou
distribuir este software, seja em forma de código-fonte ou compilado, para qualquer finalidade, comercial ou não comercial.

Para mais informações, <https://unlicense.org>