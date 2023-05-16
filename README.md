# SnowHeight
For Documentation


30.06.23

23.06.23

16.06.23

02.06.23

26.05.23
  1. Controller:
  ToDo:
  Done:
  2. Handy App:
  ToDo:
  Done:

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
  Cerate a team
Done:
  Project SnowHeight was selected
  Team was selected




General informations:

Handy App requirements:
1. Read data from the SD Card & create a chart (to check if the sensors are ok).
2. Read the EEPROM of the Controller via Bluetooth (change Meta-Data via the App, height of the station (mandatory for measurement of the snow height), duration between ultrasonic, duration between laser movement und measurement, matrix for the laser measurement as two dimensional array).
3. Send changed settings to the EEPROM 

Data stored on the SD-Card:
1. ED (Errordata) - Stores all Errors that were encountered during the usage 
of other modules and therefore has extra “Module” and “Errormessage” 
columns
2. LD (Laserdata) - Stores the distance and LaserID of each measured point in 
a laser measurement. It should be noted that LaserID and ID are two different 
fields
3. GD (Genericdata) - Stores the data collected using every data collecting 
module (except Laser module) i. e. Ultrasonic distance measurements and 
temperature, humidity and pressure of the weather sensor. Inside the File 
are extra “Module” and “Data” fields

Ebenfalls zu beachten bei APP:
Es soll in der App möglich sein zu steuern ob die Messung versetzt gestartet wird (z.B. an Baum befestigt)
app soll sich die Messpunkte ausrechnen (benötigt x y werte)
