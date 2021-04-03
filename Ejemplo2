from board import SCL, SDA
import busio
from PIL import Image, ImageDraw, ImageFont
import adafruit_ssd1306
import time

i2c = busio.I2C(SCL, SDA)
disp = adafruit_ssd1306.SSD1306_I2C(128, 64, i2c)

disp.fill(0)
disp.show()

image = Image.new('1', (128, 64))

draw = ImageDraw.Draw(image)

font = ImageFont.load_default()

#  Escribe 2 lineas texto
draw.text((50, 16),    'Hola',  font=font, fill=255)
draw.text((50, 26), 'Mundo!', font=font, fill=255)

# Muestra Texto
disp.image(image)
disp.show()
time.sleep(10)
disp.fill(0)
disp.show()
