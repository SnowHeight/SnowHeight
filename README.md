# SnowHeight
For Documentation


30.06.23

23.06.23

16.06.23
  1. Controller:
  ToDo: final test of hardware

  2. Handy-App:
  revamp bluetooth + extras
  
    

02.06.23
  1. Controller:
  ToDo:
     initial test of the hardware,
     solder pins,
     
  2. Handy App:
  ToDo:
     revise Interface
     bluetooth connection check,
     hardcoded activities revamp
     permissionsettings check
     
26.05.23
  1. Controller:
  ToDo: 
     Check missing parts,
     order missing lead battery,
     
  Done:
     missing Lead Battery ordered, 
     MicroController assembled with SD Card,
     Bluetooth-Module,Atmospheric Pressure Sensor,
     Ultrasonic Sensor
  
  Hardware:
     Ultrasonic - HCSR04,
     RTC-Timer . ZS042,
     Servomotor with attached Laser,
     Humidity + Temp. Sensor - BME280,
     SD-Card-Module
     Lead Battery - EMOS 0T 9-12 - to be delivered
     
  2. Handy App:
  ToDo: 
     navigations for read/write to sd card,
     load data, revise interface/UI,
     create functions for different activities, 
     Done:
  ToDo:
     re-check Software,
     write specification book,
     check phone app,
     Done:
     defined specifications again, 
     wrote specification book
     
  12.05.23
  1. Controller:
  ToDo:
     Check all components,
     Order missing parts,
     Software check,
  Done:
     Bluetooth-Module ordered,
     MicroController setup,
     Atmel-Studio setup,
     Project was updated to the Controller,
     Hardware: 
     Ultrasonic - HCSR04,
     RTC-Timer . ZS042,
     Servomotor with attached Laser,
     Humidity + Temp. Sensor - BME280,
     SD-Card-Module
  2. Handy App:
  ToDo:
     Create a concept
     Start with the app
  Done:    
     Concept created,
     Mockup defined for the first page
    
  05.05.23
  ToDo:
     Select a project
     Create a team
     write specifications for the project
  Done:
     Project SnowHeight was selected
     Team was selected
     Specifications defined
     
  General informations:

  Handy App requirements:
  1. Read data from the SD Card & create a chart (to check if the sensors are ok).
  2. Read the EEPROM of the Controller via Bluetooth (change Meta-Data via the App, height of the station (mandatory for measurement of the snow height), duration between ultrasonic, duration between laser    movement und measurement, matrix for the laser measurement as two dimensional array).
  3. Send changed settings to the EEPROM 

  Data stored on the SD-Card:
  1. ED (Errordata) - Stores all Errors that were encountered during the usage 
  of other modules and therefore has extra “Module” and “Errormessage” columns
  2. LD (Laserdata) - Stores the distance and LaserID of each measured point in 
  a laser measurement. It should be noted that LaserID and ID are two different 
  fields
  3. GD (Genericdata) - Stores the data collected using every data collecting 
  module (except Laser module) i. e. Ultrasonic distance measurements and 
  temperature, humidity and pressure of the weather sensor. Inside the File 
  are extra “Module” and “Data” fields

  Also, consider the following for the app:
  The app should have the option to control whether the measurement starts with a delay (for example, when attached to a tree).
  The app should calculate the measurement points based on the provided x and y values.
