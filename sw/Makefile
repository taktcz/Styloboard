MCU=attiny85

flash:
	avrdude -Cavrdude.conf -p ${MCU} -c usbasp -U flash:w:${TARGET}.hex:i 
	avrdude -p $(MCU) -c usbasp -C avrdude.conf -U lfuse:w:0xe1:m -U hfuse:w:0xdd:m -U efuse:w:0xfe:m

