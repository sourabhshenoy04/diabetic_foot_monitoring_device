# Diabetic Foot Monitoring Device


## Tech Stack

**Hardware:**
- Raspberry Pi Pico W
- NODEMCU - ESP8266
- CD74HC4067 16-Channel Analog Digital Multiplexer
- Bluetooth Module - HC-05

**Software/Tools Used:** 
- Thonny IDE
- Bluetooth Monitoring app



## Purpose:
The purpose of the "Low-Cost Diabetic Foot Monitoring Device" project is to create an affordable and accessible solution for individuals with diabetes to monitor the health of their feet. Diabetes can lead to complications such as peripheral neuropathy and poor blood circulation, which increases the risk of foot ulcers and other related issues. This project aims to provide an innovative and cost-effective way to track foot health, enabling early detection of problems and facilitating timely medical intervention.
## Benefits:
- Early Detection: Timely identification of foot health issues can prevent the development of ulcers and other complications.
- Cost-Effectiveness: The project's emphasis on affordability ensures that more individuals can benefit from this solution.
- Empowerment: Users gain greater control over their health by being informed about their foot condition and taking preventive measures through mobile.



## Working of Code:

1. **Setting Up:** The code starts by configuring the pins and communication for the Raspberry Pi Pico.

2. **Loop Begins:** The program enters a loop that will repeat indefinitely.

3. **Sensor Reading:** For each of the 16 sensor channels:
   - The code selects the sensor channel using multiplexer pins.
   - The multiplexer output is turned on.
   - The code takes multiple readings from the sensor and calculates their average voltage.

4. **Data Sending:** The average voltage is printed on the screen and sent to a Bluetooth terminal for each sensor channel.

5. **Multiplexer Off:** The multiplexer output is turned off to prepare for the next iteration.

6. **Sleep:** The program pauses for 2 seconds to allow some time between sensor readings.

7. **Loop Continues:** The loop repeats, going through the same process for all sensor channels.

8. **End of Iteration:** After all channels are processed, an empty line is sent to the Bluetooth terminal to separate the sets of data.

9. **Loop Repeats:** The loop starts over again, continuously monitoring the sensor channels and sending data.







## Screenshot of Output

![App Screenshot](./assets/pic.heic)

