# IOT-InventoryManagement
TABLE OF CONTENTS
1. INTRODUCTION………………………………………………………… Page 5-6
2. OVERVIEW OF PROJECT………………………………………………. Page 6-9
3. ALGORITHMS AND FLOW CHART ………………………………….. Page 10-12
4. CONCLUSION AND FUTURE SCOPE…………………………………. Page 13
References ………………………………………………………………… Page 14
4 | P a g e
ABSTRACT
With the development of enterprises and the constant demands of the product
diversity, traditional warehouse management models cannot meet that, due to its
heavy workload and low efficiency. This paper presents a new type of intelligent
warehouse management system - Smart Warehouse Management System based
on the IOT and expounded the principles and structure of it. This system has
great advantages compared with the traditional mode, and we expect good
prospects for its development.
By implementing the inventory management based on IOT, we eliminate the
unnecessary manpower and make it automated between the measurement and
order placement stages, thereby improving the efficiency of inventory
management. The idea utilizes the ultrasonic transducer and a processing device
with capability to connect to the Internet, to measure the inventory and send a
mail using IFTTT to the supplier and/or to the company personnel for order
placement, as well as display the present stock availability on a Web page hosted
by Thingsspeak.com.
5 | P a g e
1. CHAPTER I: INTRODUCTION
IoT-based inventory management lays a solid foundation for the digitalization of the
manufacturing ecosystems and offers both process and business benefits, including:
● Automation of inventory tracking and reporting
With RFID and IIoT, inventory managers do not need to spend time on manual tracking
and reporting. Each item is tracked and the data about it is recorded to a big data warehouse
automatically. Automated asset tracking and reporting save up to 18 hours of working time
per month and reduces the probability of human error.
● Constant visibility into the inventory items’ quantity, location, and movements
An IoT-based inventory management solution gives manufacturers precise visibility into
the flow of raw materials and components, work-in-progress and finished goods by
providing real-time updates about the status, location, and movement of the items, so that
inventory managers see when an individual inventory item enters or leaves a particular
location.
● Inventory optimization
The better inventory managers know their stock, the more likely they are to have the right
items in the right place at the right time. With the real-time data about the quantity and the
location of the inventory items, manufacturers can lower the amount of inventory on hand
while meeting the needs of the customers at the end of the supply chain.
● Identifying bottlenecks in the operations
6 | P a g e
With the real-time data about the location and the quantity of the inventory items,
manufacturers can reveal bottlenecks in the manufacturing process and pinpoint machines
with lower utilization rates. For instance, if part of the inventory tends to pile up in front
of a machine, a manufacturer assumes that the machine is underutilized and needs to be
seen to.
● Lead time optimization
By providing inventory managers with the data about the amount of available inventory
and machine learning-driven demand forecasts, solutions based on IIoT allow
manufacturers to reduce lead times.
2. CHAPTER II: OVERVIEW OF THE PROJECT
2.1 DEFINITION IOT BASED SMART FARMING SYSTEM
A typical inventory management system available in the market is built around
software, which monitors the stocks. The inventory details are updated by the workers of
the industry by various methods. One such method includes an Ultrasonic sensor. Such
type of Inventory management system is suitable for industries dealing with packaged
cartons. By establishing a shared inventory for vivid departments of the enterprise, it
allowed them to timely and efficiently maintain and control their inventory 
7 | P a g e
2.2 COMPONENTS AND MODULES
In this section, various components and Modules being used for IoT based
SMART INVENTORY MANAGEMENT SYSTEM development is discussed:
2.2.1 NodeMcu ESP8266-12e Wi-Fi development board
NodeMcu is an open source IOT platform with a deployed ESP8266-12e Wi-Fi
module in it. It supports a USB micro port for programming the NodeMcu. The em-18
module is interfaced with the NodeMcu ESp8266, the data from the em-18 RFID reader
is sent to the NodeMcu. It works on an operating voltage of 5 V, but the ESP8266-12e
module requires 3.3 V for that purpose all the required circuitry for the voltage
conversion are held in the NodeMcu board. The NodeMcu can be programmed with the
Arduino IDE and the AT commands can be easily integrated which makes coding
simpler. The NodeMcu can be programmed in two modes, STA mode, AP mode. For
simplicity, the NodeMcu is programmed in the STA mode.
2.2.2 HC-SR04 Ultrasonic Sensor
HC-SR04 Ultrasonic (US) sensor is a 4-pin module, whose pin names are Vcc,
Trigger, Echo and Ground, respectively. This sensor is a very popular sensor used in
many applications where measuring distance or sensing objects are required. HC-SR04
distance sensor is commonly used with both microcontroller and microprocessor
platforms like Arduino, ARM, PIC, Raspberry Pie etc.
Power the Sensor using a regulated +5V through the Vcc and Ground pins of the sensor.
The current consumed by the sensor is less than 15mA and hence can be directly powered
by the on board 5V pins (If available). The Trigger and the Echo pins are both I/O pins
and hence they can be connected to I/O pins of the microcontroller.
8 | P a g e
2.2.3 Breadboard
A Breadboard is a construction base for prototyping of electronics. Originally the
word referred to a literal bread board, a polished piece of wood used for slicing bread. A
modern solderless breadboard socket consists of a perforated block of plastic with
numerous tin-plated phosphor bronze or nickel silver alloy spring clips under the
perforations. The clips are often called tie points or contact points. The number of tie points
is often given in the specification of the breadboard.
The spacing between the clips (lead pitch) is typically 0.1 inches (2.54 mm). Integrated
circuits (ICs) in dual in-line packages (DIPs) can be inserted to straddle the centerline of
the block. Interconnecting wires and the leads of discrete components (such as capacitors,
resistors, and inductors) can be inserted into the remaining free holes to complete the
circuit. Where ICs are not used, discrete components and connecting wires may use any of
the holes. Typically, the spring clips are rated for 1 ampere at 5 volts and 0.333 amperes at
15 volts (5 watts). The edge of the board has male and female dovetail notches so boards
can be clipped together to form a large breadboard.
2.3 CIRCUIT DESCRIPTION & WORKING PRINCIPLE
In this circuit there is an ESP8266 Wi-Fi module connected with 2 ultrasonic sensors. The
working principle is based on storing data from sensors with the help of ESP8266 Wi-Fi
Module. The Wi-Fi module gives update of data through “Thingspeak”. The Thingspeak
link is https://thingspeak.com/channels/1222918/private_show where the channel name is
Inventory. 
9 | P a g e
Overall circuit layout
10 | P a g e
3. CHAPTER-III: ALGORITHMS & FLOWCHART &
OUTPUT GRAPHS
3.1 ALGORITHM
THE ALGORITHM OF OVERALL PROCESS: -
STEP 1: START THE PROCESS
STEP 2: CONNECT TO WIFI
STEP 3: READ THE DISTANCE OF THE CARTON FROM THE SENSOR
STEP 4: GET THE DISTANCE; USE A FORMULA TO FIND NO. OF CARTONS AND THEN
SEND DATA TO THINGSPEAK API
STEP 5: SEND EMAIL USING IFTTT IF STOCK IS LOW
STEP 6: DELAY TO 10 SECONDS
STEP 7: REPEAT STEP 4, 5 & 6 UNTIL THE PROCESS END
STEP 8: END
11 | P a g e
3.2 FLOWCHART
12 | P a g e
3.3 OUTPUT GRAPH
No. of cartons of ice cream
No. of cartons of chocolate
13 | P a g e
4. CHAPTER-IV: CONCLUSION & FUTURE SCOPE
4.1 CONCLUSION
Intelligent warehouse information management system based on the IOT get a lot
of information of different goods through the use of advanced sensor technology, and on
the basis of Internet and cloud computing technologies, achieves intelligent processing and
control of the goods in in/out of storage and cargo handling process, improving the
efficiency of warehouse management and reduce the error rate for enterprises. Also reduces
costs and the workload of staff. More and more enterprises will adopt it to get greater
assistance for the socio-economic and rapid development of enterprises.
4.2 FUTURE SCOPE
Further growth in the coming years will be possible thanks to new sensors,
more computing power, and reliable mobile connectivity. Finally, the IoT market
will grow because existing IT devices will need to be linked to the IoT. Growth in
traditional connected IT devices is admittedly moderate—about 2 percent per year
