# General Information

This project contains several repositories which contribute to the class project in the course "Smart Cities & IoT".

- (https://github.com/IoT-planthouse/planthouse-sensors)[Raspberry Pi/IoT Gateway]
  - Contains all scripts which are executed on the Raspberry Pi to read the sensor values and control the actuators
- (https://github.com/IoT-planthouse/smart-greenhouse-cloud-services)[Cloud Services]
  - Contains all code which is executed in the Azure Cloud. This mainly implements the Backend and Reasoning/Ubiquitous Layer.
  - This is deployed in one Azure Funcitons App, but consists of several own/independent functions:
  - `planthouse-backend`: Process the received sensor data and create the plan. This implements the Activity Recognition and Decision Making component
  - `read-from-database`: A simple function which enables to read the latest sensor and actuator data from the database.
  - `store-actuator-state`: This function stores the actuator state (received via topic `actuator-state` in the database)
  - `store-sensor-data`: This funciton stores the sensor data (received via topic `sensor-data` in the database)
- (https://github.com/IoT-planthouse/planthouse-ui)[WebUI]
  - Contains the Web User Interface which is accessible here: https://iot-planthouse.github.io/planthouse-ui/
- (https://github.com/IoT-planthouse/sensor-simulator)[Sensor Simulator]
  - Contains the sensor simulator
- (https://github.com/IoT-planthouse/actuator-simulator)[Actuator Simulator]
  - Contains the Actuator Simulator
- (https://github.com/IoT-planthouse/messaging)[messaging]
  - This is an informative repository, how the messaging middleware is setup and configured
 - (https://github.com/IoT-planthouse/database)[Database]
  - This is an informative repository, how the databse is setup and configured
 - (https://github.com/IoT-planthouse/test-snippets)[Test-Snippets]
  - Contains some test code. Not used for the real project
