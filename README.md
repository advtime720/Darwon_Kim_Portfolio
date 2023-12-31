# Darwon Kim - Project Portfolio

#### Personal and Academic Projects 


## \<Ultrasonic Parking Sensor>
This was my first project at UIUC during freshman year. My partner and I created a parking sensor that lights up two LEDs based on the distance from an obstruction. We decided to use the HC-SR04 ultrasonic sensor.

![project1_2](https://github.com/advtime720/Project-Portfolio/assets/150773404/d30a2e12-6f51-4756-8326-cfe4b1668fb1)

<img width="420" alt="Screenshot 2023-11-14 181413" src="https://github.com/advtime720/Project-Portfolio/assets/150773404/b0c071e6-8a0d-45c6-90f6-138c9912fd3d">
<img width="368" alt="Screenshot 2023-11-14 181438" src="https://github.com/advtime720/Project-Portfolio/assets/150773404/ec3fc3cb-7dc6-44ac-92e3-d35ba2744522">

| Components Used |
| ----------- | 
|HC-SR04 Ultrasonic Sensor|
|L7805CV Voltage Regulator|
|CD40106BE Schmitt Trigger|
|LM358N Operational Amplifier|
|LTL-4223 [Red LED], WP5603QBDL/SD/G [Blue LED]|
|Function Generator|
|Four 1N4148 Diodes|
|1 mF Capacitor|
|1k, 100 ohm resistors|

At a higher level, the circuit can be organized into 4 parts: The input, DC voltage control, amplifier, and output. The input is the ultrasonic sensor which requires an input to the "Trigger" pin in order to let the device know when to probe its field of view with an ultrasonic signal. Since we wanted the sensor to be constantly active, he connected it to a signal generator, providing an input of 130Hz with 5 Volts peak-to-peak at high-Z mode. The circuit is powered by a single 9V battery, but the ultrasonic sensor has a maximum operational voltage of 5V. This is where we used the voltage regulator to bring down the voltage to 5V for the sensor. The 5V output of the regulator will be used to power the rest of the circuit such as the op-amp and schmitt trigger. The output of the ultrasonic sensor is a PWM signal, but we needed a DC signal for the output of the circuit. We paired a shcmitt trigger with a 1mF capacitor to convert the signal to a DC voltage, which on its own is too weak to power the LEDs. So we connected it to a simple non-inverting amplifier circuit which consists of the op-amp and 2 resistors. We then hooked up the output of the op-amp to the LED and diode network. The anode of the blue LED was connected directly to the op-amp, while the red LED had four extra diodes connected in series to its anode to raise the turn-on voltage. 
<br>
<br>

 =-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=
<br>

## \<Bit-Serial Logic Processor>

For this project, my partner and I designed and implemented a bit-serial logic processor purely through hardware. 
This procesor can perform eight different, 4-bit bitwise operations. At a higher level, the processor consists of four main components:
- Register Unit
- Computation Unit
- Routing Unit
- Control Unit 

The Register Unit contains two 4-bit registers: register A and register B. The Routing Unit is used to choose which register will hold the final result. 

![full_circuit](https://github.com/advtime720/Project-Portfolio-Structure-/assets/150773404/ea5a9628-0fae-4193-9ab2-ede1d4b4a08c)
<img width="383" alt="Screenshot 2023-12-30 113049" src="https://github.com/advtime720/Project-Portfolio-Structure-/assets/150773404/0dd23c83-c0aa-4b85-a905-0a97a2cc38f3">
<img width="189" alt="routing unit layout" src="https://github.com/advtime720/Project-Portfolio-Structure-/assets/150773404/a19d7bef-e7e3-42da-9cbf-0d27b89671f0">


| key | Description |
| ----------- | ----------- |
| sections | array of sections that you want to create route for | 
| sections.component | name of the Component. No need to change it unless you want to customize the entire Component. | 
| sections.path | route for the particular section. this is the path where the particular section will be accessible | 
| sections.headerTitle | title to be shown on the top of that section page | 

- For component customization, create a component of your own inside `src/components/` and use name of that component here.


### LC-3 Calculator
### 

### (4) About Section

### (5) Skills Section

### (7) Experience Section

### (8) Projects Section

### (9) Resume Section
