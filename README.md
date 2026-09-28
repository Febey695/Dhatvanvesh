# DHATVANVESH

 Underwater Mineral Exploration System.

DHATVANVESH is a cost underwater lander built to explore the seabed. It uses geophysical sensors to find areas that might have minerals. It collects a sample from the seabed and brings it to the surface for further analysis. This system is designed to show a cycle of exploration from start to finish.

The main goal of the MVP is to prove the exploration process:

"Deploy → Descend → Reach Seabed → Scan → Detect Anomaly → Collect Sample → Recover → Analyse"


##1. Problem

Finding mineral deposits on the seabed can be very expensive. It often needs end underwater vehicles and complex deep-sea technology.

DHATVANVESH offers an cheaper solution. It is a tethered lander that can be used for initial seabed surveys.

Of trying to detect a specific element like cobalt directly with one sensor the system looks for unusual geophysical signals. If it finds something interesting it collects a sample. That sample is then examined separately to confirm what is actually there.

## 2. Proposed Solution

DHATVANVESH includes:

* A sturdy underwater lander structure

* A tether that connects the lander to the surface

* Several geophysical sensors for measuring the seabed

* Electronics that are protected from water pressure

* A mechanism to collect seabed samples

* A recovery system using the tether

* Equipment on the surface to record and analyze data


## 3. How DHATVANVESH Works

 Step 1: Deployment

The lander is attached to a surface vessel with a tether. A winch lowers it into the water.

 Step 2: Descent

The lander sinks using buoyancy. Ballast helps it go down steadily.

 Step 3: Seabed Landing

The lander reaches the seabed. Stays stable thanks to its frame and base.

Step 4: Geophysical Scanning

The sensors collect data using:

* TEM – Transient Electromagnetic

* MAG – Magnetic field measurements

* SP – potential

* CT – Conductivity and temperature sensing depending on setup

 Step 5: Data Fusion

Data from all sensors are combined to find potentially mineralized areas.

Step 6: Decision

The system follows a rule:

**GRAB - SKIP - REPEAT**

* GRAB: Take a sample if the area looks promising.

* SKIP: Move on if the signal is not strong enough.

* REPEAT: Measure again if the signal is unclear.

### Step 7: Sample Recovery

A small sample is taken from the seabed. This could be sediment, rock or a surface nodule. It is kept in a container on the lander.

### Step 8: Surface Recovery

The winch pulls the tether. The lander and sample are brought back to the surface.

### Step 9: Material Confirmation

At the surface the sample is removed and analyzed in a lab.

## 4. Mineral Detection Principle

DHATVANVESH does not claim it can detect cobalt directly.

The sensors measure geophysical properties of the seabed.

For example:

### MAG

Measures changes in the field.

### TEM

Shows how the seabed responds to pulses. This gives clues about conductivity and underground features.

### SP

Measures natural electrical differences in the seabed.

### CT / Conductivity-Temperature

Provides information about water conductivity and temperature depending on the sensor used.

Together these signals help find areas that're geophysically unusual.

So the process is:

"Sensor data → Combine measurements → Find anomaly → Collect sample → Analyze material → Confirm results"

This separates the search step from the confirmation step.

## 5. Can DHATVANVESH Detect Cobalt Directly?

No.

The MVP should not say it can find cobalt using MAG, TEM, SP or CT.

These sensors can point to a zone that might have minerals.. Only a physical sample can confirm what is actually there.

This way the system is more realistic and scientifically sound.

## 6. Underwater Pressure

Pressure increases with depth.

Approximate pressure in seawater:

* 10 m depth: 2 bar

* 30 m depth: about 4 bar

* 100 m depth: about 11 bar

* 300 m depth: about 31 bar

* 1000 m depth: about 101 bar

Water pressure doesn’t stop the lander from going down.

The lander’s electronics and structure must handle the pressure at the chosen depth.

For this college MVP a limited depth should be picked. The whole system must be tested before trying water.

## 7. Mechanical Design

The lander has:

* A strong frame to carry the load

* A stable base on the seabed

* Ballast and buoyancy components

* A pressure-resistant box for electronics

* Waterproof connections for sensors

* Mounts for sensors

* A grabber to collect samples

* A container to hold samples

* A point to attach the tether

* The tether itself

* A surface winch

The lander is designed to have buoyancy. That means it sinks.

The frame keeps it upright when it lands.

The tether controls how it goes down and comes up.

## 8. Communication

The MVP uses a connection.

Data and control flow like this:

**Surface Controller ↔ Tether ↔ DHATVANVESH Lander**

The tether gives a link for data and power if the system uses a powered cable.

Regular Wi-Fi, Bluetooth or radio signals don’t work underwater. Seawater blocks them.

Later versions could explore optical communication.

## 9. Why Communication First?

Tethered communication is used in the MVP because it gives:

* Reliable data transfer

* Control

* Easier setup

* Controlled descent and recovery

* Simpler troubleshooting

* Lower development difficulty

The main goal is to test the core system: sensing, sampling and recovery.

Adding communication too soon would add a tough challenge before the main system is proven.

## 10. Why Wireless Communication Later?

A tether has drawbacks:

* range

* Cable drag

* Hard to handle

* Less freedom to move

* Depends on surface vessel

* Hard to use in areas

After the basic system works future versions can look into acoustic or optical communication.

So:

**MVP → Tethered**

**Future → communication**

## 11. Sample Collection

The sample depends on where the lander goes.

It could be:

* Seabed sediment

* rocks

* Surface mineral material

* Nodules on the surface

The MVP uses a mechanical grabber.

The sample is stored in a container. It stays with the lander during recovery.

## 12. Detection of Nodules

For the MVP the focus is on surface and near-surface areas.

If a nodule or mineral zone affects the physical properties being measured the sensors can detect it.

Then the system decides:

**GRAB  - SKIP - REPEAT**

A real sample confirms if the signal was real.

Detection depth and clarity depend on sensor type, setup, strength, target size, seabed type and noise.

So DHATVANVESH does not claim it can see below the seabed.


This sets the base for future improvements, like deeper operation, autonomous movement, wireless communication and better mineral detection.
