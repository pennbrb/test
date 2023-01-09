# tes

I have Orange PI PC, and use Armbian Buster OS

pi@orangepipc:~$ uname -a
Linux orangepipc 5.10.12-sunxi #21.02.1 SMP Wed Feb 3 20:39:30 CET 2021 armv7l GNU/Linux

 

I have done package install of dump1090-fa and piaware by following commands:

wget https://flightaware.com/adsb/piaware/files/packages/pool/piaware/p/piaware-support/piaware-repository_5.0_all.deb  

sudo dpkg -i piaware-repository_5.0_all.deb  

sudo apt-get update  


sudo apt-get install piaware  

sudo piaware-config feeder-id xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx

sudo piaware-config allow-auto-updates yes
sudo piaware-config allow-manual-updates yes

sudo systemctl restart piaware   


sudo apt-get install dump1090-fa   

sudo reboot   
