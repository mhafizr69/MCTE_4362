----

# CONTROLLER

There are many type of controllers present in this ever advancing technology era.  
All the controllers have their own advantages to one another depending on the task.  
This table shows the specifications comparison between some of the popular type of controllers.


![Comparison between controllers](https://github.com/mhafizr69/MCTE_4342_EmbeddedSystemDesign/blob/main/Week_14/ControllerComparisonTable.png)

-----

## 1. Flight Controller

Physically, a flight controller is nothing more than a circuit board with electronic chips on them. You can compare them to the motherboard and processor in your laptop. The flight controller is the brain of a drone. A small box filled with intelligent electronics and software, which monitors and controls everything the drone does. And just like the brains of different organisms, flight controllers also vary in sizes and complexity.

<img src="https://fusion.engineering/wp-content/uploads/2020/08/Drones_compilation.jpg" width="480" height="480">

Each flight controller is equipped with different inputs and outputs for perception, controlling, and communication.

### 1.1 Perception

The flight controller is connected to a set of sensors. These sensors give the flight controller information about like its height, orientation, and speed. Common sensors include an Inertial Measurement Unit (IMU) for determining the angular speed and acceleration, a barometer for the height, and distance sensors for detecting obstacles. Just like how we perceive as humans, the drone filters a lot of this information and fuses some to get more efficient and precise information. Advanced flight controllers can sense more precisely and detect differences more quickly

### 1.2 Controlling

Aside from sensing what’s going on, a flight controller… unsurprisingly controls the motion of the drone. The drone can rotate and accelerate by creating speed differences between each of its four motors. The flight controller uses the data gathered by the sensors to calculate the desired speed for each of the four motors. The flight controller sends this desired speed to the Electronic Speed Controllers (ESC’s), which translates this desired speed into a signal that the motors can understand.

Calculating the movements, fusing and filtering the sensory information, and estimating the safety and durability of a flight is all done by an algorithm. A fancy word that is used a lot nowadays which in essence nothing more than a set of strict rules that every microchip on the board has to apply to. The most commonly used flight control algorithm is called PID control: Proportional Integral Derivative control. Within this area, there is a lot of research going on, which resulted in INDI: Incremental Nonlinear Dynamic Inversion. This algorithm reads out and reacts to incoming information way faster, therefore making the drone flight more stable.

### 1.3 Communication

A key part of a flight controller is communication. A part of the sensor’s job is to give out information that needs to be translated clearly for a pilot to read, which means efficiently. An obvious thing to communicate is its battery level, which can decide if a pilot wants to fly further or return to the charge.

But communication goes further than from flight controller to human pilot; with the entrance of auto-pilot programs in the drone industry, flight controllers need to communicate with other computer systems about its flight destination and how to get there. Communication is mostly done with wi-fi and radio frequencies right now, but cellular solutions are also already in use.

### 1.4 Types of Flight Controllers

There are a lot of different flight controllers on the market. They range from very basic to expensive systems. The types are based on users.

- FC’s for hobbyists/builders – Easy to install and perfect for people that do not want to spend large amounts of money from the get-go.
- Racing FC’s – Designed to be very lightweight, precise, and responsive. Most of them are in the €50,- or less range.
- FC’s for filming – Although mostly bought included in a drone with a camera, these flight controllers are more focussed on creating fluent shots and accessible handling for a pilot. Within this segment, Chinese company Dà-Jiāng Innovations (better known as DJI) is a household name.
- Commercial FC’s – The latest segment to evolve in the previous years. These are for the most advanced drones, capable of safe flying and transporting high-value cargo. The biggest players in this field are DJI and Pixhawk, but new flight controllers like Auterion’s Skynode and Fusion Engineering’s Fusion Reflex are also promising flight controllers in the industry.

-----

## 2. Programmable Logic Controller (PLC)

A specialized device intended to be used in applications where you have sensor inputs that need to be read and acted upon resulting in the controller outputs behaving in a defined way. It is programmable so it can behave in different ways, but it’s function is more or less limited to processing inputs and outputs in a system (usually in an industrial system). It usually consists of a CPU, memory, and Input and Output sections. The CPU can only handle a very specific set of instructions, mostly geared towards responding to inputs and controlling outputs.

<img src = "https://www.electricalchile.cl/imgplcall1.png" width = "480" height = "480">

## 3. Edge AI Controller









