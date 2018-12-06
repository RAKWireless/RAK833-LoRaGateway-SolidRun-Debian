# RAK833-LoRaGateway-SolidRun-Debian

verified on HummingBoard2 rev 1.4 and MicroSOM rev 1.5

##	Installation procedure
 
step1 : Download and install [sr-imx6-debian-stretch-cli-20180916.img.xz](https://images.solid-build.xyz/IMX6/Debian/) 

step2 : flashing image to SD card(https://wiki.solid-run.com/doku.php?id=products:imx6:overview:flashsdcard)

step3 : Clone the installer and start the installation

      $ git clone https://github.com/RAKWireless/RAK833-LoRaGateway-SolidRun-Debian.git ~/rak833-solidrun
      $ cd ~/rak833-solidrun
      $ sudo ./install.sh

step4 : make sure the mini-pcie PERST# signal(pin 22) pulled down (default high will cause rak833 function error)

step5 : Start the packet-forwarder application

      $ cd /opt/packet_forwarder/lora_pkt_fwd
      $ sudo ./lora_pkt_fwd
           

Now you have a running gateway.
