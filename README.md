
# Afterburner Toolhead Board #
![PCB](Images/PCB.jpg)

 Sơ đồ nối dây cho [Octopus](Images/Octopus_wiring.jpg)
 
    Pinout 
    24V  - PSU +V 
    GND  - PSU -V (NOT MAINS GND)
    PROBE/ABL  - Probe Signal Pin
    HE0  - Hotend Heater -V
    CT   - Chamber Thermistor Signal Pin (TH1)
    PCF  - Part Cooling Fan -V
    HEF  - Hotend Cooling Fan -V
    AGND - Hotend Thermistor -V
    TH0  - Hotend Thermistor Signal Pin (TH0)
    XES  - X Endstop Signal Pin 
    S1A  - Red Stepper Wire
    S2A  - Green Stepper Wire
    S1B  - Blue Stepper Wire
    S2B  - Black Stepper Wire 



### chamber thermistor config settings

    #######################################
    #### Enclosure Temp Sensor Section ####
    #######################################
    [thermistor chamber_temp]
    temperature1: 25
    resistance1: 10000
    beta: 3950
    
	
	[temperature_sensor enclosure_temp]
    sensor_type: chamber_temp
    sensor_pin: P0.23 #Octopus use PF5
    min_temp: 0
    max_temp: 100
    gcode_id: C
	

