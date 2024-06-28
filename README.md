Name: Satarupa Roy
Company: CODTECH IT SOLUTION
ID: CT12DS440
Domain: IoT (Internet of things)
Duration: June to August 2024
Mentor: Muzzamil Ahemed

PROJECT OVERVIEW

![Screenshot 2024-06-28 105550](https://github.com/Satarupa2002/-CODTECH-TASK-1/assets/174084276/1326185b-3e81-49b7-ac11-2cef30ddf075)



Components and brief descriptions:
DHT22 Sensor: Provides accurate measurements of temperature and humidity, essential for real-time weather monitoring.
Analog Pressure Sensor: Measures atmospheric pressure, crucial for understanding weather patterns and changes.
I2C LCD Display: Allows for easy and efficient display of sensor data, making it accessible and readable in a compact format.

Libraries Used:
Wire.h
LiquidCrystal_I2C.h
DHT.h

CODE BREAKDOWN:

-> Initialization (setup() function):

Initializes the communication with the LCD display and DHT22 sensor.
Sets up initial display messages on the LCD, such as "Weather Monitoring".

-> Main Loop (loop() function):

Sensor Readings:
Reads temperature and humidity from the DHT22 sensor using the readTemperature() and readHumidity() methods provided by the DHT.h library.
Reads atmospheric pressure from the analog pressure sensor using analogRead() function and scales the value to display in hectopascals (hPa).

Data Display on LCD:
Updates the LCD display to show:
Temperature in Celsius.
Humidity as a percentage.
Atmospheric pressure in hPa.

Rainfall Calculation:
Computes estimated rainfall based on a formula involving temperature, humidity, pressure, and predefined coefficients (a, b, c).
Displays the calculated rainfall in millimeters (mm) on the LCD.

Delay and Update:
Introduces a delay (delay(1000)) between updates to ensure the display is readable and updates occur approximately every second.

WORKING OF THE PROJECT:

In essence, the Arduino-based weather monitoring project employs sensors for temperature, humidity, and pressure, coupled with an LCD display for real-time data presentation. It provides immediate insights into local weather conditions by continuously updating the display with temperature (in Celsius), humidity (as a percentage), pressure (in hPa), and estimated rainfall (in mm). Beyond its practical use, the project serves as an educational tool, demonstrating sensor integration and data visualization through Arduino programming. It showcases the versatility of Arduino in environmental monitoring and offers potential for expansion into IoT applications or enhanced data logging capabilities.
