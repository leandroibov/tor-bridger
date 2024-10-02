
# Como usar:

sudo chmod +x bridgeson bridgeson2 bridgeson3 bridgesoff tor-bridger tor-bridger2 tor-bridger3 parator-bridger;


#### O que faz cada script

bridgeson -> Cadastra um bridge no arquivo /etc/tor/torrc do tor hidden service

bridgeson2 -> Cadastra duas bridges no arquivo /etc/tor/torrc do tor hidden service

bridgeson3 -> Cadastra três bridges no arquivo /etc/tor/torrc do tor hidden service

bridgesoff ->  Remove as bridges e retorna dados do arquivo original no arquivo /etc/tor/torrc do tor hidden service

tor-bridger -> Roteia todo o tráfego da máquina pelo tor hidden service e cadastra 1 bridge no arquivo /etc/tor/torrc do tor hidden service

tor-bridger2 -> Roteia todo o tráfego da máquina pelo tor hidden service e cadastra 2 bridges no arquivo /etc/tor/torrc do tor hidden service 

tor-bridger3 -> Roteia todo o tráfego da máquina pelo tor hidden service e cadastra 3 bridges no arquivo /etc/tor/torrc do tor hidden service 

parator-bridger -> Remove as bridges do torrc, apaga regras iptables para rotear todo o tráfego da máquina!



#### Execução, copie para o /bin

navegue até a pasta com os scripts e:

sudo cp -r bridgeson bridgeson2 bridgeson3 bridgesoff tor-bridger tor-bridger2 tor-bridger3 parator-bridger /bin;

De qualquer lugar do terminal, basta digitar os comandos:

sudo tor-bridger

Ou navegue até a pasta com os scritps e, por exemplo

sudo ./script_desejado

sudo ./tor-bridger3



##### ALERTA:

Para manter aumentar a chance de anonimidade plena, é preciso usar a técnica de mac spoofing de fabricantes, visite meu site para aprender!



## REQUISITO: OBFS4PROXY

***Instalação obfs4proxy para rotear usar as bridges no tor hidden service no Linux Debian

via apt e pacote .deb do site oficial Debian

https://packages.debian.org/buster/amd64/obfs4proxy/

***via apt


sudo echo "deb http://security.debian.org/debian-security buster/updates main" >> /etc/apt/sources.list; 


sudo apt update -y;


sudo apt install obfs4proxy -y;



***via .deb


http://security.debian.org/debian-security/pool/updates/main/o/obfs4proxy/



***Instalação



sudo dpkg -i obfs4proxy_0.0.7-4+deb10u1_amd64.deb;



#remover se precisar:



dpkg --list;


dpkg --list | grep obfs4proxy;



sudo dpkg --remove nome-do-pacote;


sudo dpkg --purge nome-do-pacote;


sudo apt-get install -f;




## CHECAR SE BRIDGES ESTÃO CONECTADAS


chmod +x checkbridges

Executar: 

./checkbridges

ou

cp -r checkbridges /bin


E bastará digitar checkbridges de qualquer localização do terminal.


Coloque o número da bridge (somente o ip), e o programará filtrará e indicará as conexões ativas.


Ele usa programas nativos do linux como /proc/net/nf_conntrack, lsof e ss!

Para rastrear com o tcpdump, use o script tcpdump-bridges!

chmod +x tcpdump-bridges

./tcpdump-bridges

Adicione o número da bridge para rastrear as conexões!

Com o wireshark faça os seguintes comandos:

ip.addr == ip_da_bridge

ip.src == ip_da_bridge

ip.dst == ip_da_bridge


##########################################################################################




# Doe monero para nos ajudar: 

### 87JGuuwXzoMGwQAcSD7cvS7D7iacPpN2f5bVqETbUvCgdEmrPZa12gh5DSiKKRgdU7c5n5x1UvZLj8PQ7AAJSso5CQxgjak

Página oficial de segurança digital:

https://traderprofissional.com.br/seguranca-digital.aspx


##### Vídeo tutorial youtube do Tor-bridger

https://www.youtube.com/watch?v=piYLFIug6ho&t=3573s




