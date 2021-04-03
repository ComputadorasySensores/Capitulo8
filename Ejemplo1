from board import SCL, SDA
import busio
import adafruit_ssd1306
i2c = busio.I2C(SCL, SDA)

# Crea la clase y define el ancho y alto de pantalla
display = adafruit_ssd1306.SSD1306_I2C(128, 64, i2c)

# Limpia la pantalla
display.fill(0)
display.show()

# Define 1 pixel en el origen 0,0
display.pixel(0, 0, 1)
# Define 1 pixel en el medio de la pantalla 
display.pixel(64, 32, 1)
# Define 1 pixel en el extremo opuesto
display.pixel(127, 63, 1)
display.show()
