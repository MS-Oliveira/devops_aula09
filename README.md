# devops_aula09  

***Primeiros passos Docker***  
Instalação em ambiente Windows  
------------------------------------------  
Link para download:   
https://download.docker.com/win/stable/Docker%20Desktop%20Installer.exe   

O link direciona para o download do arquivo .exe  

Após o download, clique no .exe e iniciará a instalação  

[![print-1.png](https://i.postimg.cc/JnSBGCMS/print-1.png)](https://postimg.cc/N970zVyx)  


Após a finalização da instalação, solicitará a reinicialização do Windows  


[![print-2.png](https://i.postimg.cc/Y9gb2HWy/print-2.png)](https://postimg.cc/9RmG1s1G)  


Depois de reiniciar o sistema aparecerá a seguinte mensagem:  


[![print-3.png](https://i.postimg.cc/02tdsQ4y/print-3.png)](https://postimg.cc/svhZPVyk)  


***Não selecione o restart e sim a opção do link (download do WSL)***  
Em seguida será direcionado para a seguinte página:  


[![print-4.png](https://i.postimg.cc/J7xjN0M5/print-4.png)](https://postimg.cc/xqkkY0kX)  


Selecione a opção baixar o pacote de atualização e em seguida inicie a instalação  


[![print-5.png](https://i.postimg.cc/g03ZnkgR/print-5.png)](https://postimg.cc/1g5tdPh5)  


Após a instalação do WSL, volte a instalação do Docker e selecione a opção restart  


[![print-6.png](https://i.postimg.cc/zBJVvwbZ/print-6.png)](https://postimg.cc/06B8Hw0c)  


Em seguida iniciará o Docker, selecione a opção sign up e será direcionado ao site para criação de usuário  


[![print-7.png](https://i.postimg.cc/QCCCkXJf/print-7.png)](https://postimg.cc/ctqddGj3)  


Após criar usuário no site volte ao Docker e digite o usuário e senha criados  


[![print-8.png](https://i.postimg.cc/ZRV0d9p9/print-8.png)](https://postimg.cc/7GJxvZBD)  


Em seguida inicie o Windows PowerShell  


[![print-9.png](https://i.postimg.cc/4NhNJ2LH/print-9.png)](https://postimg.cc/HVdCzzCT)  


# Comandos Container  


[![print-11.png](https://i.postimg.cc/Th8xLG7L/print-11.png)](https://postimg.cc/y3Tt2qzs)  



[![print-11.png](https://i.postimg.cc/Th8xLG7L/print-11.png)](https://postimg.cc/y3Tt2qzs)  

Criar um container  
pwd (anotar [caminho])  
docker run -v [caminho]:/impacta --name aula_devops -it python:3.6 bash  
Caso você tenha o problema: "the input device is not a TTY. If you are using mintty, try prefixing the command with 'winpty'"  
winpty docker run -v [caminho]:/impacta --name aula_devops -it python:3.6 bash  

Rodar um container  
docker start -ai aula_devops  

Instalar pacotes - Dentro do Container  
apt update  
apt -y install git ne  

Apagar um container  
docker rm aula_devops  

PARTE 3 - Configurando o shell  
Dentro do container clonar esse projeto  

Rodar o script prompt_setup.sh  

Lembrando que caso crie o container essa configuração deve ser refeita    

---------------------------------------------------------------------------------------  
***Fonte: Professor Thiago Kuma - Faculdade Impacta / https://github.com/thkuma/docker_linux***  





--------------------------------------------


