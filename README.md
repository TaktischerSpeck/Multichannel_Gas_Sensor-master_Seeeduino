# Multichannel_Gas_Sensor-master_Seeeduino
Seeeduino librarie for Grove Multi-Channle-Gas-Sensor

there is a compatibility problem because of the normal Library is for the Arduino.

I did the following:

Replaced "Serial" with "SerialUSB" 
In BOTH MutichannelGasSensor::get_addr_dta functions je need to insert an "delay(1)" between "Wire.endTransmission();" and "Wire.requestFrom(i2cAddress, 2);"

I already did this in this Library
