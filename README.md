# OLEDpi - Install OLED name tag on Raspberry Pi

turn on i2c with raspi-config

sudo apt install -y python3-dev python-smbus i2c-tools python3-pil python3-pip python3-setuptools python3-rpi.gpio git

i2cdetect -y 1

git clone https://github.com/adafruit/Adafruit_Python_SSD1306.git

cd Adafruit_Python_SSD1306

sudo python3 setup.py install



cd examples
python3 stats.py

copy piName.py to home & set up CRON
