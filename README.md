# upgraded-sniffle

### Hardware
```
Yaesu DR-1X 144/430 Dual Band C4FM/FM Digital Repeater      https://tinyurl.com/pecuz6y   $1679.95
NW Digital Radio Universal Digital Radio Controller II      https://tinyurl.com/k652ynm   $  89.95
CanaKit Raspberry Pi 3 with 2.5A Micro USB Power Supply     https://tinyurl.com/hmko6eg   $  41.99
SanDisk Ultra 32GB microSDHC UHS-I Card with Adapter        https://tinyurl.com/zgjctvq   $  12.94
```
### Software
```
Compass Linux Operating System                              https://tinyurl.com/mmzztt5
WB2OSZ Direwolf Soundcard Modem/TNC                         https://tinyurl.com/nkoqfn6
Linux RMS Gateway                                           https://tinyurl.com/ny7s9nk
```
##### Update Compass Image and Install Packages
```
sudo su
apt-get update
apt-get upgrade -y
apt-get install -y mg jed rsync build-essential autoconf automake libtool git libasound2-dev whois libncurses5-dev
shutdown -r now
```
##### Install Core Configuration
```
git clone https://github.com/nwdigitalradio/n7nix
cd n7nix/config
sudo su
./core_install.sh
shutdown -r now
```
##### Build / Install Direwolf Software
```
sudo apt-get -y install gpsd                                        &&
sudo apt-get -y install libasound2-dev                              &&
sudo apt-get -y install libgps-dev                                  &&
sudo apt-get -y install numlockx
```
##### Build / Install Direwolf Software
```
cd /home/pi/Desktop/                                                &&
git clone https://www.github.com/wb2osz/direwolf                    &&
cd /home/pi/Desktop/direwolf                                        &&
make                                                                &&
sudo make install                                                   &&
make install-conf
```
