# Multichannel_Gas_Sensor-master_Seeeduino
Seeeduino library for Grove Multichannel-Gas-Sensor

There is a compatibility problem because of the normal Library is for the Arduino.

I did the following:

Replaced "Serial" with "SerialUSB" 
In BOTH `MutichannelGasSensor::get_addr_dta` functions, you need to insert a `delay(1)` between `Wire.endTransmission();` and `Wire.requestFrom(i2cAddress, 2);`

I already did this in this Library
