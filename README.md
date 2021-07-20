# Converter
A DC-DC converter built around the TI LM2576
# Purpose
For the MATE robotics Explorer Category, we needed to deal with a 48V power supply.  As most of our electronics were not compatabile with this voltage we needed to convert it into something we could use.  The voltages needed were primarily 18V for our thrusters as well 5V and 12V for various electronics and servos.  Due to certain restrictions on how we could handle this conversion, size, efficiency, and simplicity were key concerns.  Because of this I elected to go with a switching power supply, specifically a buck converter, which allowed for high efficiency and widespread and available documentation.  
# Design Process
As I had never designed something like this, the first place I started was researching the theory and principles of power conversion.  After gaining a better grasp of the mechanics of the converter, I used Texas Instruments WEBENCH tool to pick the IC to power the converter as well as picking the passive components.  I then used EasyEda to design the layout and generate Gerber files.
# Key Features
1. Low Cost
2. Simple assembly with minimal SMT Components
3. Relatively small dimensions
4. Easy connections
# Implentation and Retrospective.
Due to time and COVID restraints, we were unable to validate and test the design.  We elected to go with other methods due to difficulty obtaining certain components and to decrease the amount of time building, testing, and debugging our electrical system.  I was able to procure PCBs and was able to do basic continuity checks to ensure that the device had all connections routed correctly. Looking back at the design process, some compromises were made that I would like to rectify in a redesign.  Most notable of these was the inductor I had designed for was simply to big for us to fit more than a couple in our space.  While this was not a deal breaker from a general use perspective, this fact coupled with a rather low max current supported by the IC and larger than expected power demand for our ROV left this solution inadequate for powering the entire ROV.  
