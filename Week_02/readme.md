----

# CONTROLLER

There are many type of controllers present in this ever advancing technology era.  
All the controllers have their own advantages to one another depending on the task.  
This table shows the specifications comparison between some of the popular type of controllers.


![Comparison between controllers](https://github.com/mhafizr69/MCTE_4342_EmbeddedSystemDesign/blob/main/Week_14/ControllerComparisonTable.png)

-----

 ## 1. Microcontroller

A microcontroller is a compact integrated circuit designed to govern a specific operation in an embedded system. A typical microcontroller includes a processor, memory and input/output (I/O) peripherals on a single chip.

A microcontroller is embedded inside of a system to control a singular function in a device. It does this by interpreting data it receives from its I/O peripherals using its central processor. The temporary information that the microcontroller receives is stored in its data memory, where the processor accesses it and uses instructions stored in its program memory to decipher and apply the incoming data. It then uses its I/O peripherals to communicate and enact the appropriate action.

### Core elements of a microcontroller

<details>
<summary>Processor (CPU).</summary>
  
- A processor can be thought of as the brain of the device. It processes and responds to various instructions that direct the microcontroller's function. This involves performing basic arithmetic, logic and I/O operations. It also performs data transfer operations, which communicate commands to other components in the larger embedded system.

</details>
  
<details>
<summary>Memory.</summary>
  
- A microcontroller's memory is used to store the data that the processor receives and uses to respond to instructions that it's been programmed to carry out. A microcontroller has two main memory types:
  
    1. Program memory, which stores long-term information about the instructions that the CPU carries out. Program memory is non-volatile memory, meaning it holds information over time without needing a power source.
    2. Data memory, which is required for temporary data storage while the instructions are being executed. Data memory is volatile, meaning the data it holds is temporary and is only maintained if the device is connected to a power source. 

</details>
  
<details>
<summary>I/O peripherals.</summary>
  
- The input and output devices are the interface for the processor to the outside world. The input ports receive information and send it to the processor in the form of binary data. The processor receives that data and sends the necessary instructions to output devices that execute tasks external to the microcontroller.

</details>

<details>
<summary>Analog to Digital Converter (ADC).</summary>
  
-  An ADC is a circuit that converts analog signals to digital signals. It allows the processor at the center of the microcontroller to interface with external analog devices, such as sensors.
  
</details>

<details>
<summary>Digital to Analog Converter (DAC).</summary>
  
- A DAC performs the inverse function of an ADC and allows the processor at the center of the microcontroller to communicate its outgoing signals to external analog components.

</details>

<details>
<summary>System bus.</summary>
  
- The system bus is the connective wire that links all components of the microcontroller together.

</details>

<details>
<summary>Serial port.</summary>
  
- The serial port is one example of an I/O port that allows the microcontroller to connect to external components. It has a similar function to a USB or a parallel port but differs in the way it exchanges bits.

</details>

### Well known Microcontroller

- Arduino boards by Arduino

<img src = "https://techatronic.com/wp-content/uploads/2022/01/different-types-of-Arduino-boards.jpeg" width = "755" height = "409">

-----

## 2. Single-Board Computer

A single-board computer (SBC) is a computer which is a complete computer in which a single circuit board comprises memory, input/output, a microprocessor and all other necessary features. However, unlike a personal computer, it does not rely on expansions for other functions. A single-board computer reduces the system's overall cost as the number of circuit boards, connectors and driver circuits are all reduced.

### Advantages:

- Very small.
- The computing power very efficient.
- Self-contained.

### Disadvantages:

- Can be quite expensive.
- GPIO output power constraints on some boards.
- Limited options for interacting with external sensors.

### Well known SBC

- SBC by Raspberri Pi

<img src = "https://opensource.com/sites/default/files/raspberry-pi-boards-2020.png" width = "650" height = "693">

----

## 3. Edge AI Controller

Edge AI is the deployment of AI applications in devices throughout the physical world. It’s called “edge AI” because the AI computation is done near the user at the edge of the network, close to where the data is located, rather than centrally in a cloud computing facility or private data center.

Edge AI is typically used for inference, whereas cloud AI is utilised to train new algorithms. Inferencing algorithms use a fraction of the computing power and energy that training methods do. As a result, well-designed inferencing algorithms are sometimes implemented in edge devices using current CPUs or even less powerful microcontrollers. In other circumstances, highly efficient AI processors boost inferencing performance while lowering power consumption or doing both.

The advantages of Edge AI from the conventional Cloud AI are:

<details>
<summary>Reduced latency/higher speeds.</summary>
  
- Inferencing is performed locally, eliminating delays in communicating with the cloud and waiting for the response.

</details>

<details>
<summary>Reduced bandwidth requirement and cost.</summary>
  
- Edge AI reduces the bandwidth and associated costs for shipping voice, video and high-fidelity sensor data over cell networks.

</details>
  
<details>
<summary>Increased data security.</summary>
  
- Data is processed locally, which reduces the risk that sensitive data is stored in the cloud or intercepted in transit.

</details>
  
<details>
<summary>Improved reliability/autonomous technology.</summary>
  
- The AI can continue to operate even if the network or cloud service goes down, which is critical for applications such as autonomous cars and industrial robots.

</details>
  
<details>
<summary>Reduced power.</summary>
  
- Many AI tasks can be performed with less energy on the device than would be required to send the data to the cloud, thus extending battery life.

</details>

### 📷 Some Edge AI controllers in the market

- Jetson Series by NVidia

<img src = "https://developer.nvidia.com/sites/default/files/akamai/embedded/images/jetson-family/jetson-family-devkit-devzone-853x298.jpg" width = "900" height = "320">

- SK-TDA4VM by Texas Instrument
 
<img src = "https://www.ti.com/content/dam/ticom/images/products/ic/processors/evm-boards/j721exskg01evm-angled.png:large" width = "480" height = "320">
 
 ------
 
## 4. Flight Controller

Physically, a flight controller is nothing more than a circuit board with electronic chips on them. You can compare them to the motherboard and processor in your laptop. The flight controller is the brain of a drone. A small box filled with intelligent electronics and software, which monitors and controls everything the drone does. And just like the brains of different organisms, flight controllers also vary in sizes and complexity.

<img src="https://fusion.engineering/wp-content/uploads/2020/08/Drones_compilation.jpg" width="480" height="480">

Each flight controller is equipped with different inputs and outputs for perception, controlling, and communication.

<details>
<summary>Perception</summary>

The flight controller is connected to a set of sensors. These sensors give the flight controller information about like its height, orientation, and speed. Common sensors include an Inertial Measurement Unit (IMU) for determining the angular speed and acceleration, a barometer for the height, and distance sensors for detecting obstacles. Just like how we perceive as humans, the drone filters a lot of this information and fuses some to get more efficient and precise information. Advanced flight controllers can sense more precisely and detect differences more quickly
</details>
  
<details>  
<summary>Controlling</summary>

Aside from sensing what’s going on, a flight controller… unsurprisingly controls the motion of the drone. The drone can rotate and accelerate by creating speed differences between each of its four motors. The flight controller uses the data gathered by the sensors to calculate the desired speed for each of the four motors. The flight controller sends this desired speed to the Electronic Speed Controllers (ESC’s), which translates this desired speed into a signal that the motors can understand.

Calculating the movements, fusing and filtering the sensory information, and estimating the safety and durability of a flight is all done by an algorithm. A fancy word that is used a lot nowadays which in essence nothing more than a set of strict rules that every microchip on the board has to apply to. The most commonly used flight control algorithm is called PID control: Proportional Integral Derivative control. Within this area, there is a lot of research going on, which resulted in INDI: Incremental Nonlinear Dynamic Inversion. This algorithm reads out and reacts to incoming information way faster, therefore making the drone flight more stable.
</details>
  
<details>  
<summary>Communication</summary>

A key part of a flight controller is communication. A part of the sensor’s job is to give out information that needs to be translated clearly for a pilot to read, which means efficiently. An obvious thing to communicate is its battery level, which can decide if a pilot wants to fly further or return to the charge.

But communication goes further than from flight controller to human pilot; with the entrance of auto-pilot programs in the drone industry, flight controllers need to communicate with other computer systems about its flight destination and how to get there. Communication is mostly done with wi-fi and radio frequencies right now, but cellular solutions are also already in use.

</details>

### Types of Flight Controllers

There are a lot of different flight controllers on the market. They range from very basic to expensive systems. The types are based on users.

- FC’s for hobbyists/builders – Easy to install and perfect for people that do not want to spend large amounts of money from the get-go.
- Racing FC’s – Designed to be very lightweight, precise, and responsive. Most of them are in the €50,- or less range.
- FC’s for filming – Although mostly bought included in a drone with a camera, these flight controllers are more focussed on creating fluent shots and accessible handling for a pilot. Within this segment, Chinese company Dà-Jiāng Innovations (better known as DJI) is a household name.
- Commercial FC’s – The latest segment to evolve in the previous years. These are for the most advanced drones, capable of safe flying and transporting high-value cargo. The biggest players in this field are DJI and Pixhawk, but new flight controllers like Auterion’s Skynode and Fusion Engineering’s Fusion Reflex are also promising flight controllers in the industry.

-----

## 5. Programmable Logic Controller (PLC)

A specialized device intended to be used in applications where you have sensor inputs that need to be read and acted upon resulting in the controller outputs behaving in a defined way. It is programmable so it can behave in different ways, but it’s function is more or less limited to processing inputs and outputs in a system (usually in an industrial system). It usually consists of a CPU, memory, and Input and Output sections. The CPU can only handle a very specific set of instructions, mostly geared towards responding to inputs and controlling outputs.

<img src = "https://www.electricalchile.cl/imgplcall1.png" width = "480" height = "480">


