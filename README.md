# Tempsensor
INEL4206-030 Final Proyect in which we need to create a serverless code that worked reading temperature and constantly publishing values to a cloud.

# Introduction
This project consists of having a ESP32 that reads the temperature in a room and sends that information to a cloud.

- Create a code for the ESP32 that reads the temperature of the room with a thermistor.
- Connect the esp32 to the wifi
- Create an online cloud server
- Create teh keys for the server to control the cloud server
- Buy a domain to put the IP direction of teh cloud CPU
- Enter from your remote server and download node-red
- Open node-red create a workflow that receives the information and uploads the information to the server
- Create an interface 
-Add teh wifi library and pubsubclient
-He Siri

# Needed Materials

- ESP32 Microcontroller
- Breadboard
- Jumper cables
- USB 2.0 - USB-mini cabke
- Thermistor
- Sensor

# Software needed
To work with the project you need this softwares

- Github
- Visual Studio
  - C/C++ compiler
  - Platformio
- Node-red

# Reference Materials


# Services
For this project you need to use this services

- AWS server (this is the clound in which you upload your work)
- Whois (it's the domain in which you use your IP address)

# Instructions

## Requirements to start
Before starting the project, you need to have completed all the requirements

- Have the ESP32 microcontroller with all the materials needed
- Have VS Code with all the compilers needed installed
- The AWS server to upload to the cloud.

## Instruction to upload the code to the cloud

- Create a code that constantly reads the temperature in Celcius and Fahrenheit.
  - Include equation which takes the values ADC, in other words the voltage from there will give the values for Celcius and Fahrenheit.
  - In teh thermistor circuit you must include a resistance of 10k that connects to the output voltage of 3.3v
- Connect the ESP32 to the wifi
  - Must include the library wifi
  - Specify the name and password to connect to the internet
- Create a server in the cloud
  - With AWS create an account and purchase a remote machine 
  - Create an Ubuntu and add a static IP address that will be used later.
- Create the safe keys (private and public)
  - Generate a random key that will be public and save it next to the key of the virtual machine
  - Safe the private key in SSH format in your computer and rename it as private
  - With this you can control your server from your computer
- Buy a domain
  - Choose a name for the domain and proceed to buy it
  - Once you buy the domain, put the static IP address
- Enter to the server through your computer
  - Once initialized start the download of node-red to the server
  - Download the admin packs comes with node-red
  - Open node-red in google utilizing tempsensor.space:1880
- Open node-red
  - Once node-red start creating the workflow of how to receive the data to the MQTT broker
  - It publish it graphically with the help of the dashboard
- Create an inteface
  - The interface is created by adding groups and creating subgroup in those groups
  - Assign a graph to each group and then you can visualize it by typing in google tempsensor.spcae:1880/ui/
- Return to the code
  - Add the library pubsubclient with the code for the MQTT connect to the internet for it to connect to the ESP32
- Hey Siri
  - Will be developed in node-red

