# Custom Lab Oven: Build and Characterization

To complete high temperature laboratory experiments, [our lab](http://www.ece.ualberta.ca/~iyer/lab.html) required a custom uniform heating solution. Utilizing the build techniques and components found at [Whizoo.com](https://Whizoo.com), a regular toaster oven was outfit with better sealing, insulation, and control (using the Controleo3).

Being a custom-built tool rather than a commercial product, it is important to [characterize](#characterization) it's performance. This website will serve as reference.

## The Build
Our build was very similar to the one depicted at [Whizoo.com](https://www.whizoo.com/reflowoven) where they have shown the steps in much greater detail. Ours documentation is to show the quality of work, and that the steps of the guide were followed accurately to produce a quality product.

### 1. Sealing
The outer case was removed and the interior and exterior cracks were sealed using a silicone sealant rated for °C. The elements themselves were quite loose, so the sealant fixed them in-place. This is one of several steps to mitigate heat loss from the interior of the oven.


![Inner Seal](https://github.com/brentlabs/brentlabs/blob/gh-pages/2_inner_seal.png?raw=true)
![Outer Seal](https://github.com/brentlabs/brentlabs/blob/gh-pages/1_outer_seal.png?raw=true)

### 2. Controleo3 Case Assembly
While the sealant of the previous step dried, the Controleo3 case was assembled. This involved some drilling and bending of a small aluminum sheet (this is how the case will attach to the oven later).


![Cont Case](https://github.com/brentlabs/brentlabs/blob/gh-pages/3_cont_case.png?raw=true)

### 3. Relay Setup
Three solid state relays (SSR) were backed with a thermally-conductive pad (the blue stuff) and fixed to an aluminum plate, which will act as a heatsink. These interface the AC with the DC (microcontroller) and allow each element of the build to be controlled independently. There is one SSR for each element: the boost element (will be added in another step), the bottom, and the top. 


![SSR](https://github.com/brentlabs/brentlabs/blob/gh-pages/4_ssr.png?raw=true)

### 4. Preparing the DC Power Supply
Wire was stripped, ends crimped, and heat shrink tubing applied. This power supply (PS) will be mounted inside the oven alongside the SSR assembly. It simply powers the Controleo3 with its 5V output.


![DC PS](https://github.com/brentlabs/brentlabs/blob/gh-pages/5_dc_ps.png?raw=true)

### 5. Applying Heat Reflective Tape
The oven door in particular is subject to heat loss through the glass. To mitigate this loss, high quality Reflect-A-Gold tape is applied. This works by reflecting radiant heat. While not shown in the below photo, additional tape was applied inside the oven.


![Gold Tape](https://github.com/brentlabs/brentlabs/blob/gh-pages/6_gold_tape.png?raw=true)

### 6. Installation of Floor Shield and Boost Element
Floor and Tunnel Shield II was applied to the interior bottom, top, and back of the oven - another tactic to mitigate heat loss. Once the bottom shielding was in-place, a 350W boost element could be installed.


![Boost_Flr_Shield](https://github.com/brentlabs/brentlabs/blob/gh-pages/7_boost_flr_shld.png?raw=true)

### 7. Fixing SSR Assembly and Thermocouple Install
The SSR assembly from step 3 was bolted to the bottom of the oven. There is a gap between the sidewall of the oven and the aluminum plate that the SSR are fixed to in order to accomodate cables and ceramic fiber insulation in a later step. Additionally, a thermocouple was installed into the oven (white cable with blue stripes) and fixed in-place by sealing it with the silicone sealant as in step 1. Similarly, the wires of the boost element were sealed as well, helping prevent heat loss through the hole they are fed through and fixing them (and thus, the element) from moving.


![SSR_Mounted](https://github.com/brentlabs/brentlabs/blob/gh-pages/8_ssr_mounted.png?raw=true)

### 8. AC and DC Wiring
The high voltage wiring was completed by re-using wires from the original oven components. These correspond to the top SRR inputs. Not shown: The Controleo3 was wired with 4 inputs- one from each SRR, and a common input to all of them. The wires from the 5V DC power supply in step 4 were also connected to the microcontroller, as were the thermocouple leads.


![AC_Wiring](https://github.com/brentlabs/brentlabs/blob/gh-pages/9_ac_wiring.png?raw=true)
![DC_Wiring](https://github.com/brentlabs/brentlabs/blob/gh-pages/10_dc_wiring.png?raw=true)

### 9. Mounting and Basic Test of Controleo3
The Controleo3, now wired and fixed in its enclosure as prepared in step 2, was mounted to the front of the oven without obstructing the door. With all wiring done and hardware mounted, it was time to test the system. Plugging the oven in, the Controleo3 started and offered its menu. 'Test' was selected, and each element was tested independently and verified to be working.


![Cont_Mounted](https://github.com/brentlabs/brentlabs/blob/gh-pages/11_cont_mounted.png?raw=true)

### 10. Access Ports
This is where we deviate from the Whizoo guide. Our oven requires access ports for data cables. To ensure a smooth run for the cable between inside and outside the oven, we use 1/2" copper pipe which was perforated to reduce its thermal mass (we don't want too much loss to escape the interior through the pipe). Large holes had to be drilled/nibbled (using a nibbling tool- extremely handy) in the walls of the oven, through the SRR aluminum plate, and the outer chassis. Only one port depicted; the other is simpler as it does not have to pass by any electronics.


![Pipe](https://github.com/brentlabs/brentlabs/blob/gh-pages/12_pipe.png?raw=true)

### 11. Ceramic Fiber Insulation 
Ceramic fiber insulation was wrapped around the exterior oven walls (before the chassis was put back on). Holes had to be created to accomodate the access port pipes as well as a lead from the top element.


![Insul](https://github.com/brentlabs/brentlabs/blob/gh-pages/13_insul.png?raw=true)

### 12. Putting Things Together
The outer chassis was replaced over the newly insulated oven. The access port pipes were aligned with holes created in the chassis and then sealed using the silicone gasket maker. Sealing them in-place will make troubleshooting/modifying difficult in the future, but it is important that they do not move. 


![Port_Sideview](https://github.com/brentlabs/brentlabs/blob/gh-pages/15_port_sideview.png?raw=true)

While the silicone seal cured, the servo motor arm mechanism was installed, as was a latch onto the oven door handle. The motor can be programmed to open the door should cooling be required.


![Servo](https://github.com/brentlabs/brentlabs/blob/gh-pages/14_servo.png?raw=true)

### 13. Finished Lab Oven and "Oven Score"
Some finishing touches included:
- Fabric gasket was lined around the frame of the oven door to address heat loss in that area.
- More Reflect-A-Gold tape was used inside the oven, especially on the sidewalls.
- High temperature flue tape was used around some of the outer edges of the exterior of the oven.
- Ceramic fiber wool to insulate the access ports.


![Final_Build](https://github.com/brentlabs/brentlabs/blob/gh-pages/final_build.png?raw=true)

Once the build guide had been satisfied, the learning cycle was performed to ...

Our oven score:


![Oven Score](https://github.com/brentlabs/brentlabs/blob/gh-pages/x_ovenscore.png?raw=true)

## Characterization
Characterization of oven performance is done through the software of the Controleo3 itself, and independently using temperature labels distributed throughout the oven.

### 1. Controleo3 Intelligent Tuning and Oven Score
For a detailed description of how the Controleo3 tunes itself and the criteria for the oven score, please see [Whizoo.com](https://Whizoo.com/intelligent).

Whizoo build oven score:



![Oven score](https://github.com/brentlabs/brentlabs/blob/gh-pages/ovenscore_temp.png?raw=true)



To summarize, this indicates...

### 2. Temperature Labels
Using 5-point temperature labels...
