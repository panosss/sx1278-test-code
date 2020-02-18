# sx1278-test-code
Test code for sx1278 with STM32F030F4P6 .
This is a working code (code taken from https://github.com/wdomski/SX1278-example).
It 's a transmitter (I already have a working and tested receiver with ESP8266).

It 's working. BUT there are missed packets: if the transmitter transmits a 100 packets (messages) the reciever will receive only 10 of them.

The modifications I have made:
1. In main.c, master = 1; So I don't have to use a MODE_Pin.
2. In main.h, I have modified the pins
3. In main.c, in the loop ('while (1) {') I have simplified the code as it 's only transmitter.


In 1st the picture you can see how I have setted the pins of STM32. 
In the 2nd the picture you can see how the two ICs are connected.

![sx1278-test-code](https://user-images.githubusercontent.com/6674193/72550890-66dc7900-389c-11ea-9fcd-241da2b11519.png)


![sx1278-test-code-stm32f0](https://user-images.githubusercontent.com/6674193/72552646-fdf70000-389f-11ea-95fa-264ffa0d08ff.png)
