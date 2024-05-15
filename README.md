# PCB-Design-Application
# Aim
To design a 2 flasher circuit as a PCB design application.

# Software required
Eagle

# Procedure
1.Open a new schematic file within your project.</br>
2.Use the libraries provided in EAGLE or create custom libraries if necessary.</br>
3.Place components onto the schematic sheet by using the 'Add' tool.</br>
4.Connect the components using the 'Net' tool.</br>
5.Label nets appropriately to ensure clarity</br>
6.Once routing is complete, perform a ERC to ensure there are no errors and save the schematic.</br>
7.Click on the 'Generate/Switch to Board' icon to create a board from your schematic.</br>
8.EAGLE's board layout editor allows you to place components, route traces, and define board shapes.</br>
9.Arrange components on the board to optimize space usage and minimize signal interference.</br>
10.Route traces to connect components according to your schematic.</br>
11.Use the various routing and editing tools provided by EAGLE to ensure proper routing and avoid design rule violations.</br>
12.Once routing is complete, perform a design rule check (DRC) to ensure there are no errors and save the board layout.</br>
13.Go to File > CAM Processor and set up CAM jobs to generate Gerber files for your PCB layers.</br>
14.Verify generated files to ensure they contain all necessary information.</br>
15.Save the generated manufacturing files.</br>

# Theory

A 2 LED flasher circuit is a simple electronic configuration often built using a 555 timer IC or a basic transistor-based astable multivibrator. The fundamental operation revolves around the generation of a square wave, which alternately drives two LEDs. In a 555 timer-based design, the IC is configured in astable mode, where it continuously switches states between high and low. This causes the output pin to oscillate, turning on and off the LEDs connected to it. Each LED is connected in series with a current-limiting resistor to prevent excessive current flow. The timing of the oscillation, and consequently the flashing rate, is determined by the external resistors and capacitors connected to the 555 timer. In a transistor-based design, two transistors are cross-coupled through capacitors, forming a regenerative feedback loop that produces an oscillating output. When one transistor conducts, it lights up the corresponding LED and turns off the other transistor, causing the alternate LED to light up in the next cycle. This continuous alternation results in the flashing effect. Adjusting the resistor and capacitor values in either circuit type can vary the flashing frequency. These circuits are widely used in decorative lighting, signal indicators, and educational electronics projects due to their simplicity and effectiveness.

### Working 

1.To build a 2 LED flasher circuit using a 555 timer IC, start by gathering the necessary components: a 555 timer IC, two LEDs, two 470Ω resistors, a 10kΩ resistor, a 100µF capacitor, a 10µF capacitor, a breadboard, and connecting wires. 
2.Begin by placing the 555 timer IC on the breadboard, ensuring it straddles the central groove. Connect pin 1 of the 555 timer to the ground rail and pin 8 to the positive power rail. Also, connect pin 4 (RESET) to the positive power rail. 
3.Next, configure the timing components by connecting a 10kΩ resistor between pins 7 (DISCHARGE) and 8 (VCC), and then connect a wire between pins 7 and 6 (THRESHOLD). Attach a 10µF capacitor between pin 6 and ground. 
4.For the LED setup, connect the anode of the first LED to pin 3 (OUTPUT) of the 555 timer, and place a 470Ω resistor in series with the cathode of this LED to ground. Similarly, connect the anode of the second 5.LED to the junction of the 10kΩ resistor and pin 7, with another 470Ω resistor in series with the cathode of the second LED to ground. 
6.Power up the circuit with a 9V battery or suitable power supply, and the LEDs will alternately flash, creating the desired flasher effect.

# Circuit Diagram
![2-led-flashing](https://github.com/mukeshkumar1110/PCB-Design-Application/assets/152305679/05c89a32-b3a1-4163-9b4c-6d0417137551)

# Output
### Schematic diagram
![Screenshot 2024-05-15 155612](https://github.com/mukeshkumar1110/PCB-Design-Application/assets/152305679/78968d85-fd87-4929-aa3a-0e9dc0812cab)

### Layout diagram
![Screenshot 2024-05-15 160458](https://github.com/mukeshkumar1110/PCB-Design-Application/assets/152305679/89a04b5d-4508-4892-9372-a69fb2cc2d0d)

# Result
Thus the 2 flasher circuit is design as a PCB application successfully.

