# Washroom-Availability-Indication-System
This washroom availability system facilitates efficient usage of toilets in public spaces/ residential buildings.

# Objectives of the project:

Facilitating efficient usage of toilets and bathrooms

Displaying the availability of the cubicles on a GUI in real time

Using in-built algorithms to direct the user to the nearest washroom/ bathroom

Providing the building maintenence administrator the root access to allow for easy display of out of service cubicles

# How does this work?

This project includes concepts from multiple domains such as Internet of Things, Database Management Systems , App Development, UX/UI Design and working with sensors. 

The IR sensors connected to each cubicle door are set to a value of binary 1 when the door is closed, this triggers the ESP module to send the signal to the web server, which using a web app/ mobile application can be set to "Occupied" , or "Available" when it is binary 0.

Here's the block diagram of the proposed model:

![221880808-b89cd1a9-1af6-4b47-944a-c7c3f5bac0a7](https://user-images.githubusercontent.com/78555241/232109538-76f8cd36-39f1-431d-87bd-cd7099a5c17d.png)

As seen above, the project uses 2 microcontroller boards, Arduino UNO for reading the input from the installed Infrared sensors, and an ESP8266 module attached to the Arduino via serial communication to coneect the system to an online database (ThingSpeak).

The status of the availability, as mentioned above can be displayed through a mobile application, I had used Android Studio to create 2 different apps, one for the client and one for the admin. However, this could vary based on your needs.

# Components Required:

Arduino UNO 

ESP8266 Module

Some sensor to read the door closing (Infrared sensors are used here)

A ThingSpeak free account

Connecting wires to tie everything together
