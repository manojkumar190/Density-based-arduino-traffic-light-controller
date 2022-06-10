# Density-based-arduino-traffic-light-controller

ABSTRACT

Congestion is a serious issue due to vehicular traffic. One of the known causes of traffic congestion is the amount of time spend waiting for the red light to change to green. The changing of traffic light is hard-coded and it is not reliant on traffic volume. There is therefore need to simulate and optimize traffic control to better accommodate density-based traffic rather than time based. This system attempts to lessen possibilities of traffic jams brought about by traffic lights to a reasonable degree. This project, a density-based traffic control system is been implemented to solve this problem. The system entails programming an Arduino using Arduino integrated development environment (IDE) to enable traffic lights give the right of access to the road by selecting the lane with the high number of cars. The traffic lights are modified to chip away at an auspicious premise until there is a signal identified by the infrared sensors. The sensor identifies an object (i.e. a vehicle, a motorcycle etc) and signals the Arduino to control the traffic lights for its individual path. Once there is no sign identified by any of the four sensors the traffic lights keep on dealing with an auspicious premise

1.1	Purpose
One of such over-stretched infrastructure is the road, a circumstance which has resulted to increase in traffic. In spite of the fact that traffic lights have dependably been utilized for controlling the movement of traffic (pedestrian or automobile), traffic management in many real urban areas around the globe has kept on being a subject of concern. A traffic light is a signaling device which controls a traffic flow at road intersections. It consists of three basic lights which include red, yellow and green. Red signal is used to halt traffic from proceeding; yellow signal alerts vehicles for brief stop, while green signal alerts vehicles for procession in the indicated directions. Traffic congestion is a situation that happens on road networks in which vehicles travel slower than usual due to the increased physical use of vehicles (traffic) on the road at that moment. Also known as traffic jam, traffic congestions may result from roads being blocked, bad roads, accidents on the road, lack of proper traffic light system to control vehicles, inappropriate driving by road users etc. This would make the journey longer due to the slow movement of the traffic and increased queuing of vehicles. Urban communities started to make traffic tenets to minimize crashes, while traffic flags and cops were utilized to coordinate option to proceed at major urban convergences. Traffic control development in urban streets has aided easy movement and use of automobile in mega cities. Most of the major roads have effective traffic control system, which has facilitated easy flow of vehicles in urban regions. Railroads were invented serving as a temporary solution to the developing issue of street traffic control. However, this creates congestion at terminals inside urban communities. Therefore, the aim of this study is to design a density-based traffic control using Arduino in order to solve the problem of traffic congestion.


1.2	Scope

In the design and construction of this system all components work simultaneously. The system works just as a typical traffic light system. The uniqueness of this is in the event that the thickness of vehicles in a specific path of the road is high. At that point, the sensor in that specific path turns out to be low else it is read as a high signal. The signal from the IR (Infrared) is used by the system to control the traffic jamming of the lane. In the event that we get a low signal from any of these sensors, at that point the green LED shines to that specific way and gives a red to every other way. The Arduino IDE is programmed using C language.

CHAPTER 2
Design/Implementation



2.1 	Introduction

In this project, an Arduino based Traffic Light Controller system is designed. It is a simple implementation of traffic lights system but can be extended to a real time system with programmable timings, pedestrian lighting etc


2.2 	Design Approach

In this system, we will use IR sensors to measure the traffic density. We have to arrange one IR sensor for each road; these sensors always sense the traffic on that particular road. All these sensors are interfaced to the microcontroller. Based on these sensors, controller detects the traffic and controls the traffic system. The main heart of this traffic system is microcontroller. IR sensors are connected to the PORT C (PC0, PC1, PC2, and PC3) of the microcontroller and traffic lights are connected to PORT B and PORT D. If there is a traffic on road then that particular sensor output becomes logic 0 otherwise logic 1. By receiving these IR sensor outputs, we have to write the program to control the traffic system. If you receive logic 0 from any of these sensors, we have to give the green signal to that particular path and give red signal to all other paths. Here continuously we have to monitor the IR sensors to check for the traffic.

2.3 	Proposed System

	The traffic lights will provide instructions to the users (drivers and pedestrians) by displaying lights of standard color. The three colors used in traffic lights are Red, Yellow and Green.

	The system must be used to control the traffic lights for smooth and safe movement of traffic

![image](https://user-images.githubusercontent.com/66869358/173084086-98411079-6664-438f-820e-5dac31d9b8f0.png)
2.3.1 	Economic Feasibility

	The traffic light issue is obviously a critical problem that worries citizens and governments. The influence of low efficient conventional traffic system affects the economic, health, financial, and environmental domains.

By using this smart traffic management system, we can reduce pollution and also average waiting time

2.3.2 	Technical feasibility:
   
The smart light traffic control system is composed of two separate devices: the traffic master controller and the handheld portable controller. Fig. 3 shows the hardware implemented circuit of the smart traffic controller using the Proteus software. The traffic master controller is mounted with the traffic lights at the roads intersection and is responsible for the lighting transition and their timing slots. Its implemented design circuit includes: the PIC 16F877A microcontroller, the three lights (red, green, and yellow) of the traffic lights A and B associated to the roads 1 and 2, the two lights (red and green) for the traffic light R and L associated with the deflection to the right and left in the direction of roads 3 and 4, the two IR receivers to measure the traffic volume, the XBee transmitter system, and other basic components. The traffic master controller provides the duration and the schedule of the two configurations and their dedicated phases for different modes of traffic. It determines the status of the different lights by commanding the triggered switches connected to the PIC ports. The microcontroller is also connected to IR detectors whose output voltages are responsible of shifting the counter of the cars arriving at the intersection. Finally, the XBee module receives the command orders form the portable controller and calls the corresponding emergency subroutines. The portable controller commands the traffic master controller by means of XBee transceiver that communicates wirelessly with the other XBee component. A PIC 16F877A constitutes the hardware core of the portable controller. It is connected, in addition to XBee, to the buttons EA and EB that start up the emergency subroutines. An LCD screen is employed to notify the user if the mode of emergency is operating and which emergency procedure is currently running. We propose also a password of 6 digits formed by the combinations of 4 digits from 1 to 4 in order to supply the portable controller by a certain security level. The total number of arrangements is 4096 possibilities. The role of security code is to prevent unauthorized persons from accessing to the smart light system.


2.3.3 	Operational feasibility 

This section describes the calibrations and the sampling rate of various sensors used in Precision agriculture system. 
	We will implement traffic light controller using smart traffic management, which means the traffic lights keeps updating based on traffic near the signal count and vehicle flowing under the traffic light per time unit and use different intervals of green/red light





2.4 	Overview of software
	

	Oak Ridge National Lab is already working on a slice of the problem. Researchers there are using overhead cameras and roadway sensors to identify gas guzzling commercial trucks in traffic. AI and machine learning algorithms identify the least-efficient vehicles, track their path and speed and change the traffic signals ahead of the vehicles.  This eliminates much of the inefficient starting and stopping at intersections and minimizes fuel consumption.

	Creation of such a system, especially for dense urban corridors and sprawling exurbs, can greatly improve energy and sustainability impacts.

	This is critical as our transportation portfolio will continue to have a heavy reliance on gasoline-powered vehicles for some time.



2.5	Hardware Specification 
	
	ATmega8 microcontroller.
	4 X HC-SR04 ultrasonic sensors
	4 X Red LEDs
	4 X Green LEDs
	4 X Yellow LEDs
	4 X 10K ohm resistors
	Jumper cables
	Breadboards


2.6	Software Requirements

	PROTEUS
The Proteus Design Suite is a proprietary software tool suite used primarily for electronic design automation. The software is used mainly by electronic design engineers and technicians to create schematics and electronic prints for manufacturing printed circuit boards.


	ARDUINO
The open-source Arduino Software (IDE) makes it easy to write code and upload it to the board. It runs on Windows, Mac OS X, and Linux. The environment is written in Java and based on Processing and other open-source software.
This software can be used with any Arduino board.





2.7 Summary

	The main purpose of this project is, if there will be no traffic on the other signal, one shouldn’t wait for that signal. The system will skip that signal and will move on the next one.
Arduino is the main part of this project and it will be used to read from ultrasonic sensor HC-SR04 and calculate the distance. This distance will tell us if any vehicle is near the signal or not and according to that the traffic signals will be controlled.
The main task was to avoid use of delay because we have to continuously read from the ultrasonic sensors and also at the same time, we have to control signals which requires the use of delay function.
So, we have used the timer one library which is used to repetitively measure a period of time in microseconds and at the end of each period, an interrupt function will be called. In this function, we will read from the sensors and in the loop function, we will control the traffic signals.









CHAPTER 3
Result and Analysis / Testing

3.1	Density Based Traffic Light Control System Circuit Design

This is the complete circuit diagram of the system. On the left you can see push buttons acting as IR sensors. Each
pair of push button is numbered according to the road they are sensing. On the right side the signals are given which
are interfaced with the port 1 of the controller .Below is the LCD interfaced with the microcontroller which will
show weather the signals are operating normally or for the dense case
This is the complete circuit diagram of the system. On the left you can see push buttons acting as IR sensors. Each
pair of push button is numbered according to the road they are sensing. On the right side the signals are given which
are interfaced with the port 1 of the controller .Below is the LCD interfaced with the microcontroller which will
show weather the signals are operating normally or for the dense case
This circuit consists of 4 IR sensors, atmega8 microcontroller, 4 traffic lights.
IR transmitter looks like an LED. This IR transmitter always emits IR rays from it. The operating voltage of this IR transmitter is 2 to 3v. These IR (infra-red) rays are invisible to the human eye. But we can view these IR rays through camera.
IR receiver receives IR rays that are transmitted by IR transmitter. Normally IR receiver has high resistance in order of mega ohms, when it is receiving IR rays the resistance is very low. The operating voltage of IR receiver also 2 to 3V. We have to place these IR pair in such a way that when we place an obstacle in front of this IR pair, IR receiver should be able to receive the IR rays. When we give the power, the transmitted IR rays hit the object and reflect back to the IR receiver.
Instead of traffic lights, you can use LEDs (RED, GREEN, YELLOW). In normal traffic system, you have to glow the LEDs on time basis. If the traffic density is high on any particular path, then glows green LED of that particular path and glows the red LEDs for remaining paths. In normal traffic system, we allow the traffic for a time delay of 1 minute for each path. Here 10k ohm resistor is used to drop the voltage otherwise IR transmitter may get damaged.

![image](https://user-images.githubusercontent.com/66869358/173084211-b7736be5-71dc-49d8-95c0-833d0872b0fd.png)

Arduino Code

Code:
#define F_CPU 8000000UL
#include <avr/io.h>
#include <util/delay.h>

#define R1 PB0
#define Y1 PB1
#define G1 PB2

#define R2 PB3
#define Y2 PB4
#define G2 PB5

#define R3 PD5
#define Y3 PD4
#define G3 PD3

#define R4 PD2
#define Y4 PD1
#define G4 PD0

int main(void)
{
  DDRB = 0xff;
  DDRD = 0xff;
  DDRC = 0x00;
  
  PORTB = 0x00;
  PORTD = 0x00;
  
  while(1)
  {
  if((PINC&0x01) == 0x01)
  {
  PORTB |= (1<<G1);
  PORTB |= (1<<Y2);
  PORTD |= (1<<R3);
  PORTD |= (1<<R4);

  }
  else if((PINC&0x02) == 0x02)
  {
  PORTB |= (1<<R1);
  PORTB |= (1<<G2);
  PORTD |= (1<<Y3);
  PORTD |= (1<<R4); 

  }

  else if((PINC&0x04) == 0x04)
  {
  PORTB |= (1<<R1);
  PORTB |= (1<<R2);
  PORTD |= (1<<G3);
  PORTD |= (1<<Y4);

  }

  else if((PINC&0x08) == 0x08)
  {
  PORTB |= (1<<Y1);
  PORTB |= (1<<R2);
  PORTD |= (1<<R3);
  PORTD |= (1<<G4);

  }

  else
  {
    PORTB = 0x00;
  PORTD = 0x00;

  PORTB |= (1<<G1);
  PORTB |= (1<<Y2);
  PORTD |= (1<<R3);
  PORTD |= (1<<R4);
   _delay_us(500000);

  PORTB = 0x00;
  PORTD = 0x00;

  PORTB |= (1<<R1);
  PORTB |= (1<<G2);
  PORTD |= (1<<Y3);
  PORTD |= (1<<R4);
   _delay_us(500000);

  PORTB = 0x00;
  PORTD = 0x00;

  PORTB |= (1<<R1);
  PORTB |= (1<<R2);
  PORTD |= (1<<G3);
  PORTD |= (1<<Y4);
  _delay_us(500000);

  PORTB = 0x00;
  PORTD = 0x00;
  PORTB |= (1<<Y1);
  PORTB |= (1<<R2);
  PORTD |= (1<<R3);
  PORTD |= (1<<G4);
  _delay_us(500000);
  PORTB = 0x00;
  PORTD = 0x00;
  }   
  }
}


![image](https://user-images.githubusercontent.com/66869358/173084574-52f7c52e-b16e-45c8-9b10-763f07bc55e4.png)

.3 	How to Connect the Circuit 

•	Connect four IR sensors to PORT C.
•	Connect LEDs to PORT B and PORT D.
•	Arrange all this LED’s same as like traffic lights.
•	Arrange one IR sensor for each road.
•	Run the Arduino code in Arduino code in Arduino IDE and find the location ending with  .hex shown after compiling the code.

![image](https://user-images.githubusercontent.com/66869358/173084821-56667b0d-c065-48f7-aaeb-aa236a7a95fd.png)


 
Figure 3.3 Compiled Result of Code

•	Copy the link address highlighted part in the above diagram and open edit properties of the Arduino and paste the copied file in the Program file section of it.

![image](https://user-images.githubusercontent.com/66869358/173084851-ac4c22b9-a14f-4236-a074-c9f9dd91ec0c.png)

 
Figure 3.4 Arduino Properties
•	Save the changes and then Run the circuit in normal mode.
•	Now you can see the normal traffic system based on time basis.
•	Now if we increase density/ place any obstacle in front of any IR sensor, then the system allows the traffic of that particular path by glowing GREEN light
![image](https://user-images.githubusercontent.com/66869358/173084870-76b6a4e6-7bbd-4fe7-ac0d-d67405c1f0e6.png)


3.4      Testing of the Circuit

Case 1: Density of traffic is high in A direction at the signal then green light will be shown at A direction and remaining sides will have Red/ Yellow.



 ![image](https://user-images.githubusercontent.com/66869358/173084899-89858caa-cb77-4214-9af6-d30db331725d.png)

Figure 3.5 Green light glowing in side A with high Density









Case 2: Density of traffic is high in B direction at the signal then green light will be shown at B direction and remaining sides will have Red/ Yellow.

 ![image](https://user-images.githubusercontent.com/66869358/173084935-e37ea4fa-cadd-4c08-91ac-94d372fd818b.png)

Figure 3.6 Green light glowing in side B with high Density



Case 3: Density of traffic is high in C direction at the signal then green light will be shown at C direction and remaining sides will have Red/ Yellow.

 
Figure 3.7 Green light glowing in side C with high Density
Case 4: Density of traffic is high in D direction at the signal then green light will be shown at D direction and remaining sides will have Red/ Yellow.
 ![image](https://user-images.githubusercontent.com/66869358/173084950-e034b3fd-771f-42dd-b0ff-d536681dc245.png)
Figure 3.8 Green light glowing in side D with high Density


Case 5: If density is high in any two of the directions, then the green light will be shown for 
the two directions in the order of clockwise directions.

Responsive Time
The response time of the sensor is the time taken for the sensor to produce an output. This is the time it takes once it detects an obstacle and sends a signal to the Arduino and changes the traffic light color for execution. The result obtained here is in agreement with the report of Table 3.1 shows the average response time and Figure 10 is the pictorial chart of the time.

Number of Attempts	Time (s)
1	0.32
2	0.41
3	0.44
4	0.31
5	0.31
6	0.32
7	0.54
8	0.54
9	0.29
10	0.39
Mean	0.387
Table 3.1
3.5      Summary

The density-based traffic control system has been designed, constructed and tested to ensure validation of its function and operations. By using this system configuration, we try to reduce the possibilities of traffic jams, caused by traffic lights. Number of passing vehicle in the fixed time slot on the road decide the density range of traffics and on the basis of vehicle density calculation, microcontroller decide the traffic light delays

Discussion 
There are some limitations in this model
•	IR sensors sometimes may absorb normal light also. As a result, traffic system works in improper way.
•	IR sensors work only for fewer distances.
•	We have to arrange IR sensors in accurate manner otherwise they may not detect the traffic density. 




