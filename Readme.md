# Issues found while testing the first version

* Resisor package is 0201, change it to 0603
* I2C pins are located in a invalid pin. Correct location is:
   * TWD0 SPI\_SDA => PA3 
   * TWCK SPI\_CLK PA4
* I2C pull up resistors are missed (4k7)
* SPI pins are located in a invalid pin. Correct location is:
    * MISO => PA12
    * MOSI => PA13
    * SPCK => PA14
* DS18B20 can be serialized. Hot/Cold temperature of each radiator could use the same bus
