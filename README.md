## Adafruit LTC4311 I2C Extender / Active Terminator PCB

<a href="http://www.adafruit.com/products/4756"><img src="assets/4756.jpg?raw=true" width="500px"><br/>
Click here to purchase one from the Adafruit shop</a>

PCB files for the Adafruit LTC4311 I2C Extender / Active Terminator.

Format is EagleCAD schematic and board layout
* https://www.adafruit.com/product/4756

### Description

I2C stands for Inter-Integrated-Circuit communications, its meant for short distances on a PCB or subassembly. But, hey, we're engineers and we like to push the limits of technology, right? So why not try to have I2C run over a meter long cable, or even longer? Well, if you try to do that you'll quickly find that the length of the cable adds capacitance and resistance that slows down the open-drain pullups used in I2C, making it hard to use 100KHz+ clock speeds. You could try slowing down your I2C clock to 1 KHz...or you could use an Adafruit LTC4311 active terminator like this one!

Using this board is easy: connect it to your I2C bus at the beginning of the chain (if you don't have a massively long cable, you can also try at the end of the chain). When the chip is powered and enabled, it will watch the SCL and SDA lines. When it sees them being pulled up through the I2C resistors, it will activate and dump in some current to give it a boost thru to the top power rail.

You can now achieve much faster data rates without having to noodle with resistors, and over long cables. We ran a 400 KHz OLED over 3 meters of phone wire with ease. With a 100KHz signal, we even ran a BME680 over 100 feet of Ethernet (about 3000pF round trip!), and had an OLED display the sensor details.

Runs with any bus voltage, from 1.6V to 5.5V and up to 400 KHz SCL speed, with cables up to 4000pF. No special firmware, software, or configuration required. Simply plug the power, ground, SCL and SDA connectors into your bus and watch as your rise times magically turn sawtooths into square waves.

To get you going fast, we spun up a custom made PCB in the STEMMA QT form factor, making it easy to interface with. The STEMMA QT connectors on either side are compatible with the SparkFun Qwiic I2C connectors. This allows you to make solderless connections between your development board and the LTC4311 or to chain it with a wide range of other sensors and accessories using a compatible cable.

### License

Adafruit invests time and resources providing this open source design, please support Adafruit and open-source hardware by purchasing products from [Adafruit](https://www.adafruit.com)!

Designed by Limor Fried/Ladyada for Adafruit Industries.

Creative Commons Attribution/Share-Alike, all text above must be included in any redistribution.
See license.txt for additional details.
