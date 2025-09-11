---
layout: project
type: project
image: img/pressure_sens_schem.jpg
title: "Vacuum Pressure Sensor"
date: 2024
published: true
labels:
  - Sensors
  - Arduino
summary: "I developed a pressure sensor arduino device tha reads and displays the atmospheric pressure readings"
---

<div class="text-center p-4">
  <img width="500px" src="../img/pressure_img.jpeg" class="img-thumbnail" >
  <video width="320" controls>
        <source src="../img/pressure_sens.mp4" type="video/mp4">
  </video>
</div>




At my job for the University of Hawaii at Manoa's Physics and Astronomy laboratory, I created a electronic pressure sensor. The sensor is used by the Physics department in measuring the air pressure of their vacuum chamber, which they use to run space related experiments, one of which involved particle smaples collected from an interplanetary body.

I began by connecting two OLED displays with an Arduino 2560, and once I got the driver installed and communicating between the Arduino and OLEDs, I tested and connected MKS pressure sensors with the Arduino. I had to utilize a Max3232 so that communication between the Arduino and the MKS sensors. Additionally, I had to solder on wires between the Max3232 and a DB9 connector for easier connectivity. Once I was sure the sensors were communicating the correct pressure data to the Arduino, and that the Arduino was displaying on the OLEDs the data sent by the sensors, I drew up schematics and soldered all the different components together. I received a 3D-printed holding box that was able to hold my pressure sensor module together neatly.


Here is some code that illustrates how we read values from the line sensors:
```cpp
//  Take returned pressure sensor text and trim out data readings only
String parse_string( String data ) {
  int ack_index = data.indexOf("ACK");
  int semicolon_index = data.indexOf(';');
  if (ack_index != -1 && semicolon_index != -1) {
    return data.substring(ack_index + 3, semicolon_index);
  } else {
    return "Invalid";
  }
}
```

You can learn more at my [Github repo](https://github.com/komochristian/Pressure_Sens_Disp).
