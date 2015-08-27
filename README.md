# SolarDisplay
Project to create a Raspberry Pi based LED display to show real time solar panel production.

This project uses Python web scraping (lxml and requests libraries) to grab the current and daily production numbers from the solaredge.com user portal every 5 minutes. This specific project won't be useful to anyone without a Solar Edge inverter, but the concepts and techniques should work for any other web-based values.

Those numbers are then used to drive a couple 4-digit I2C alphanumeric LED displays (Adafruit product 2157) to show the current and daily production values. Current NTP time will also be displayed on a 3rd display for convenience.

All of this is housed in a 3D printed enclosure for desktop or wall mount display. Power is provided directly to the RPi with a micro USB charger which then directly drives the LED displays. A 1A or greater charger is required.
