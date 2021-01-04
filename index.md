# Custom Lab Oven: Build and Characterization

To complete high temperature laboratory experiments, [our lab](http://www.ece.ualberta.ca/~iyer/lab.html) required a custom uniform heating solution. Utilizing the build techniques and components found at [Whizoo.com](https://Whizoo.com), a regular toaster oven was outfit with better sealing, insulation, and control (using the Controleo3).

Being a custom-built tool rather than a commercial product, it is important to [characterize](#characterization) it's performance. This website will serve as reference.

## The Build
Our build was very similar to the one depicted at [Whizoo.com](https://www.whizoo.com/reflowoven) where they have shown the steps in much greater detail. Ours are shown to show the quality of work.

### 1. Sealing
The outer case was removed and the interior and exterior cracks were sealed using a silicone sealant rated for °C. The elements themselves were quite loose, so the sealant fixed them in-place. This is one of several steps to mitigate heat loss from the interior of the oven.


![Inner Seal](https://github.com/brentlabs/brentlabs/blob/gh-pages/2_inner_seal.jpg?raw=true)
![Outer Seal](https://github.com/brentlabs/brentlabs/blob/gh-pages/1_outer_seal.jpg?raw=true)

### 2. Controleo3 Case Assembly
While the sealant of the previous step dried, the Controleo3 case was assembled. This involved some drilling and bending of a small aluminum sheet (this is how the case will attach to the oven later).


![Cont Case](https://github.com/brentlabs/brentlabs/blob/gh-pages/3_cont_case.jpg?raw=true)

### 3. Relay Setup
Three solid state relays (SSR) were backed with a thermally-conductive pad (the blue stuff) and fixed to an aluminum plate, which will act as a heatsink. These interface the AC with the DC (microcontroller) and allow each element of the build to be controlled independently. There is one SSR for each element: the boost element (will be added in another step), the bottom, and the top. 


![SSR](https://github.com/brentlabs/brentlabs/blob/gh-pages/4_ssr.jpg?raw=true)

### 4. Preparing the DC Power Supply
Wire was stripped, ends crimped, and heat shrink tubing applied. This power supply (PS) will be mounted inside the oven alongside the SSR assembly. It simply powers the Controleo3 with its 5V output.


![DC PS](https://github.com/brentlabs/brentlabs/blob/gh-pages/5_dc_ps.jpg?raw=true)

### 5. Applying Heat Reflective Tape
The oven door in particular is subject to heat loss through the glass. To mitigate this loss, high quality Reflect-A-Gold tape is applied. This works by reflecting radiant heat. While not shown in the below photo, additional tape was applied inside the oven.


![Gold Tape](https://github.com/brentlabs/brentlabs/blob/gh-pages/6_gold_tape.jpg?raw=true)

### 6. Installation of Floor Shield and Boost Element
Floor and Tunnel Shield II was applied to the interior bottom, top, and back of the oven - another tactic to mitigate heat loss. Once the bottom shielding was in-place, a 350W boost element could be installed.


![Boost_Flr_Shield](https://github.com/brentlabs/brentlabs/blob/gh-pages/7_boost_flr_shld.jpg?raw=true)

### 7. Fixing SSR Assembly and Thermocouple Install
The SSR assembly from step 3 was bolted to the bottom of the oven. There is a gap between the sidewall of the oven and the aluminum plate that the SSR are fixed to in order to accomodate cables and ceramic fiber insulation in a later step. Additionally, a thermocouple was installed into the oven (white cable with blue stripes) and fixed in-place by sealing it with the silicone sealant as in step 1. Similarly, the wires of the boost element were sealed as well, helping prevent heat loss through the hole they are fed through and fixing them (and thus, the element) from moving.


![SSR_Mounted](https://github.com/brentlabs/brentlabs/blob/gh-pages/8_ssr_mounted.jpg?raw=true)


## Characterization
Characterization of oven performance is done through the software of the Controleo3 itself, and independently using temperature labels distributed throughout the oven.

### 1. Controleo3 Intelligent Tuning and Oven Score
For a detailed description of how the Controleo3 tunes itself and the criteria for the oven score, please see [Whizoo.com](https://Whizoo.com/intelligent).

Our oven score:



![Oven score](https://github.com/brentlabs/brentlabs/blob/gh-pages/ovenscore_temp.png?raw=true)



To summarize, this indicates...

### 2. Temperature Labels
Using 5-point temperature labels...
