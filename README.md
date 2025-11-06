# Voltage-divider-5v-input-and-3.37v-output-
This is a simple Voltage Divider for a 5v signal that converts it into 3.37v for ESP-32

## Sketch:

- R1 = 2 KΩ
- R2 = 330 Ω
- R3 = 100 Ω
- R4 = 5.1 KΩ
- ○ = a pin/point where you can connect your kable
- (Rx) = resistor
- "|" and "─"  = powerline/connection



**curcuit:**
```txt
(GND)
|
(R4)
|
○───(R3)───(R2)───(R1)───○
(3.37v            (5v signal input)
signal
output)
```

## Explenation:

At the beggining we have the **5v signal input** then this signal will go through 3 Resistors in series (one 2KΩ, one 330Ω and one 100Ω). 
Then we reached the output pin, this is where you connect your signal with your ESP-32 Module.
Then the pin is connected with a single 5.1KΩ Resistor that is connected to Ground.


**Warning**:
Always check with a multimeter if you did everything right. to do this you simply connect your COM probe to the GND connection behind the 5.1KΩ and the Red one to the output pin.
if everything is right you should get 3.37v as result.
