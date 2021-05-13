# ME 193 Project 6: Using the DHT sensor on the Pico
Using the DHT11 temperature humidity sensor with the Raspberry Pi Pico
The DHT11 sensor uses a capacitive humidity sensor and a thermistor to measure the surrounding environment's air, and the sensor can be integrated with a microcontroller to measure the humidity and temperature.

**Setup:**
The digital output of the DHT11 sensor was connected to GP28 on the Pico. The SDA and SCL pins of the OLED display were conencted to GP8 and GP9 on the Pico. The DHT 11 and OLED diplay were connected to ground and the 3.3V from the Pico board to complete the circuit.

<img src="https://user-images.githubusercontent.com/78379722/118066328-87bbbe00-b36c-11eb-80c2-2c1540b057d2.jpg" width="600" height="600"> 

**Code for this project:**
1. **SSD1306.py**: contains code for the OLED display library. A SSD1306 OLED driver with I2C and SPI interfaces was used
2. **dht.py**: contains code for the DHT11 sensor library
3. **main.py**: the main code run for this project that collects the outputs from the sensor and displays it on the OLED screen and the shell window
