# Inter Integrated Circuit (I2C)

# Abstract
This article describes the detailed design and implementation of I2C slave circuitry for write and read operations from a latch unit, implemented in a 0.6μm CMOS technology. For the purpose of demonstration, the I2C circuit was designed and fabricated in 0.6µm CMOS technology.

# Introduction
An I2C protocol is one of the serial communication protocols that are used for chip to chip communication. Similar to the I2C protocol, SPI and UART are also used for chip to chip communication. The I2C is the short form of Inter-Integrated Circuit, a type of bus, which was designed and developed by Philips in 1980 for inter-chip communication. I2C is adopted by a lot of vendor companies for the chip to chip communication.

Features of I2C protocol:
 ## In I2C only two buses are required for the communication, the serial data bus (SDA) and serial clock bus (SCL). 
Each component in I2C bus is software addressable by a unique address, this unique address is used by the master to communicate with a particular slave. 
Always a master and slave relationships exist at all times in I2C. 
In I2C, communication is started by the master. 
The master can send data to a slave or receive data from a slave - slaves do not transfer data between themselves.
I2C is the 8-bit oriented serial bidirectional communication, there are following speed mode in I2C 
