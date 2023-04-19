 
# Projeto MQTT Broker 
Criação de um ambiente de desenvolvimento, utilizando o Vagrant em conjunto com o VirtualBox, e utilizando o equipamento IOT Raspberry pico W.
Foram definidos alguns requesitos, e implementados no projeto.



# Índice  
1. [Introdução](#projeto-mqtt-broker)  
2. [Tech Stack](#tech-stack)  
    1. [Sub paragraph](#subparagraph1)  
3. [Another paragraph](#paragraph2)  

## Screenshots  

![App Screenshot](https://github.com/PaivaX/MQTT-vagrant/blob/main/share/logo.png?raw=true)

## Tech Stack  

**Client:** ubuntu, paho MQTT  

**Server:** ubuntu, MQTT Mosquitto

**Raspberry Pico:** MycroPython

## Features  

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

Ir para o directório do projeto  

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

## Environment Variables  

To run this project, you will need to add the following environment variables to your .env file  
`API_KEY`  

`ANOTHER_API_KEY` 

## Acknowledgements  

- [Awesome Readme Templates](https://awesomeopensource.com/project/elangosundar/awesome-README-templates)
- [Awesome README](https://github.com/matiassingers/awesome-readme)
- [How to write a Good readme](https://bulldogjob.com/news/449-how-to-write-a-good-readme-for-your-github-project)

## Relatório  

If you have any feedback, please reach out to us at fake@fake.com

## License  

[MIT](https://choosealicense.com/licenses/mit/)
