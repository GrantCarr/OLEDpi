# OLEDpi - Install OLED name tag on Raspberry Pi 3

turn on i2c with raspi-confi

sudo apt install -y python3-dev python-smbus i2c-tools python3-pil python3-pip python3-setuptools python3-rpi.gpio git

i2cdetect -y 1

git clone https://github.com/adafruit/Adafruit_Python_SSD1306.git

cd Adafruit_Python_SSD1306

sudo python3 setup.py install

cd ..

git clone https://github.com/GrantCarr/OLEDpi.git

sudo crontab -e

add: @reboot python3 /home/pi/OLEDpi/piName.py

# OLEDpi - Install OLED name tag on Raspberry Pi 4

turn on i2c in raspi-config

sudo apt install python3-dev python-smbus i2c-tools python3-pil python3-pip python3-setuptools python3-rpi.gpio git

sudo pip3 install Adafruit_BBIO

i2cdetect -y 1

git clone https://github.com/adafruit/Adafruit_Python_SSD1306.git

cd Adafruit_Python_SSD1306

sudo python3 setup.py install

cd ..

git clone https://github.com/GrantCarr/OLEDpi.git

cd OLEDpi

python3 piName.py

sudo crontab -e

add: @reboot python3 /home/pi/OLEDpi/piName.py


