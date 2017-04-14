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
##### Build / Install Direwolf Software
```
sudo apt-get install gpsd                                           &&
sudo apt-get install libasound2-dev                                 &&
sudo apt-get install libgps-dev                                     
```
##### Build / Install Direwolf Software
```
cd /home/pi/Desktop/                                                &&
git clone https://www.github.com/wb2osz/direwolf                    &&
make
sudo make install


mkdir /home/pi/Desktop/direwolf/build                               &&
cd /home/pi/Desktop/direwolf/build                                  &&


mkdir /home/pi/aprswx/                                              &&
cd /home/pi/aprswx/                                                 &&
git clone git://git.osmocom.org/rtl-sdr.git                         &&
mkdir /home/pi/aprswx/rtl-sdr/build/                                &&
cd /home/pi/aprswx/rtl-sdr/build/                                   &&
cmake ../ -DINSTALL_UDEV_RULES=ON                                   &&
make                                                                &&
sudo make install                                                   &&
sudo ldconfig                                                       &&
cd /home/pi/
```
