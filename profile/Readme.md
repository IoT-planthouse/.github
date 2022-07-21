# General Information

This project contains several repositories which contribute to the class project in the course "Smart Cities & IoT".

- [Raspberry Pi/IoT Gateway](https://github.com/IoT-planthouse/planthouse-sensors)
  - Contains all scripts which are executed on the Raspberry Pi to read the sensor values and control the actuators
- [Cloud Services](https://github.com/IoT-planthouse/smart-greenhouse-cloud-services)
  - Contains all code which is executed in the Azure Cloud. This mainly implements the Backend and Reasoning/Ubiquitous Layer.
  - This is deployed in one Azure Funcitons App, but consists of several own/independent functions:
  - `planthouse-backend`: Process the received sensor data and create the plan. This implements the Activity Recognition and Decision Making component
  - `read-from-database`: A simple function which enables to read the latest sensor and actuator data from the database.
  - `store-actuator-state`: This function stores the actuator state (received via topic `actuator-state` in the database)
  - `store-sensor-data`: This funciton stores the sensor data (received via topic `sensor-data` in the database)
- [WebUI](https://github.com/IoT-planthouse/planthouse-ui)
  - Contains the Web User Interface which is accessible here: https://iot-planthouse.github.io/planthouse-ui/
- [Sensor Simulator](https://github.com/IoT-planthouse/sensor-simulator)
  - Contains the sensor simulator
- [Actuator Simulator](https://github.com/IoT-planthouse/actuator-simulator)
  - Contains the Actuator Simulator
- [messaging](https://github.com/IoT-planthouse/messaging)
  - This is an informative repository, how the messaging middleware is setup and configured
- [Database](https://github.com/IoT-planthouse/database)
  - This is an informative repository, how the databse is setup and configured
- [Test-Snippets](https://github.com/IoT-planthouse/test-snippets)
  - Contains some test code. Not used for the real project
