# Remote Control Car Project 🚗🔧

## 📌 Overview
Me and my friend like thingies that move, so it becomes natural for us to build a RC car.
This project fulfilled our interest and also improved our problem solving and creative thinking, especially in the engineering field.
it also enchanced our hands-on experience with tools.

The RC car is controlled via an 27 MHz 4CH RC module(transmitter and receiver), with a wood chassis, plastic over and used double battereies to power 2 dc motors.  
Through this project, we explored **circuit wiring, steering design, sketching, experimenting design and troubleshooting hardware problems**.  

**Outcome:** A fully functional RC car capable of forward/reverse driving, turning.

---

## 🛠️ Materials & Components
### Electronics
- 27Mhz 4CH RC transmitter
- 27Mhz 4CH RC receiver
- 3-6V DC motors  
- Wires    
- AA Batteries  

### Mechanical
- Wood Chasis
- Cardboard
- Plastic Cover
- 4 × Wheels with rubber tires  
- Axles 
- Heat shrnk tubing 
- Screws, nuts, and nails  

### Tools & Software
- Soldering iron   
- Hot glue gun   
- Pliers
- Multipurpose wire stripper.
- Scissor
- Pencil
- Sketching book

- ---

<div align="center">
  <img src="Images/sketch.jpg" alt="Sketch" width="600"/>
  <p><em>rough sketches of steering system designs.</em></p>
</div>

<br>
<br>

<div align="center">
  <img src="Images/v1.jpg" alt="steering v1" width="600"/>
  <p><em>version 1 of steering system, failed due to invalid dimension and insufficient space to implement.</em></p>
</div>

<div align="center">
  <img src="Images/v2.jpg" alt="steering v2" width="600"/>
  <p><em>version 2 of steering system, improved with more space and easy to implement, howver failed due to motor unable to produce enoygh torque when being placed too far in the back.</em></p>
</div>

<div align="center">
  <img src="Images/v3.jpg" alt="steering v3" width="600"/>
  <p><em>version 3 of steering system, improved from v2, added suppports, made everything more compact and effcicient, put motor closer to ensure enough torque</em></p>
</div>

---

## 🧩 Challenges & Problems Faced

During the build process, we encountered some challenges.  
Each problem required troubleshooting and iteration, which provided valuable hands-on learning.

### ⚡ Steering Issues
- **Problem:** The steering motor unable to produce enough torque to overcome friction.  
- **Cause:** 2 AA battery does not produce enough voltage.  
- **Solution:** Soldered two battery holders in series, so that the car has 4 AA batteries (6V), which maxes out the motors potential, which turned out to be successful.  

---

### 🖥️ Unable to turn on
- **Problem:** The receiver fails to turn on.  
- **Cause:** AFter checking all related conections, we found out that the V+ wire had poor connection.
- **Solution:** We resoldered the V+ wire and made sure all wires had proper protection and are well secured. 

---

