hashs sha256

81197c8bdf3010bd9531e308850094f1500fe00c2d83095a11a2d5c55bd3e293  bridgesoff

a4cdc47677086f9314044f32e33b1e57b3dae00d8ac0e2e8bd1bf6f9dff36417  bridgeson

f87ea4c37ae39eacf4bb23ba654a3c31e4c34913a223110585762d688a984608  bridgeson2

58dd61b045b17499827713f386d8a73a6e0d28d34ea2a43e41768fca7f6f4cb5  bridgeson3

56b2b292530e8b55dd4648eb02dfdc2315826a525bcd2ffdd987abb91cc1a5a1  parator-bridger

730e267cf900a58f94cd4174a3bb48f306dca78f00fde0df615ee20b081b7cd8  tor-bridger

b41047c971a128b27b7fec7dd234cbab1067d815b7fa64a245a1fb3e719a66b3  tor-bridger2

de2713ce1682a9029ef5b1967a765beafc340b0aa018e61b9bddcfc950e0a871  tor-bridger3



##########################################################################################

Como usar:

sudo chmod +x bridgeson bridgeson2 bridgeson3 bridgesoff tor-bridger tor-bridger2 tor-bridger3 parator-bridger;


##########################################################################################

O que faz cada script

bridgeson -> Cadastra um bridge no arquivo /etc/tor/torrc do tor hidden service

bridgeson2 -> Cadastra duas bridges no arquivo /etc/tor/torrc do tor hidden service

bridgeson3 -> Cadastra três bridges no arquivo /etc/tor/torrc do tor hidden service

bridgesoff ->  Remove as bridges e retorna dados do arquivo original no arquivo /etc/tor/torrc do tor hidden service

tor-bridger -> Roteia todo o tráfego da máquina pelo tor hidden service e cadastra 1 bridge no arquivo /etc/tor/torrc do tor hidden service

tor-bridger2 -> Roteia todo o tráfego da máquina pelo tor hidden service e cadastra 2 bridges no arquivo /etc/tor/torrc do tor hidden service 

tor-bridger3 -> Roteia todo o tráfego da máquina pelo tor hidden service e cadastra 3 bridges no arquivo /etc/tor/torrc do tor hidden service 

parator-bridger -> Remove as bridges do torrc, apaga regras iptables para rotear todo o tráfego da máquina!



##########################################################################################
Execução, copie para o /bin

navegue até a pasta com os scripts e:

sudo cp -r bridgeson bridgeson2 bridgeson3 bridgesoff tor-bridger tor-bridger2 tor-bridger3 parator-bridger /bin;

De qualquer lugar do terminal, basta digitar os comandos:

sudo tor-bridger

Ou navegue até a pasta com os scritps e, por exemplo

sudo ./script_desejado

sudo ./tor-bridger3


##########################################################################################

ALERTA:

Para manter aumentar a chance de anonimidade plena, é preciso usar a técnica de mac spoofing de fabricantes, visite meu site para aprender!



##########################################################################################
