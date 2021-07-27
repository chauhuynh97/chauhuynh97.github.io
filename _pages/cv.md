---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* Masters in Electrical Engineering, University of Washington graduating June 2022
* B.S. in Electrical and Computer Engineering, Seattle University graduated 2019


Work experience
======
* Assembly Technician at Technical and Assembly Services Corporation (TASC), January 2020 – August 2020
** Soldered surface-mount and through-hole electronic components, assembled electronic parts, and performed functionality tests and
quality inspections on industrial and commercial items.
* Mathematics Tutor at Seattle University, January 2017 – June 2019
** Reviewed assigned materials to strengthen students’ comprehension, developed students’ abiity to self-learn.

Skills
======
* Languages: C++, C#, Python, C, MATLAB, MySQL, SQLite, F#, VHDL, MIPS Assembly
* Relevant coursework: Linear Algebra, Calc and Multivariable Calc, Probability and Statistics, Differential Equations, Data
Structures, Computing Systems, Object-Oriented Development, Design and Analysis of Algorithms

Projects
=====

* Data Logger for KiloWatts for Humanity, September 2018 – June 2019
** Improved an existing Raspberry-Pi-based data logger to increase feature parody with expensive commercial data loggers needed by
a non-profit organization, KiloWatts for Humanity (KWH), reducing production costs by 60%.
** Designed and implemented a data-handling structure in MySQL to store, transmit, and retransmit data to a live data site in
case of unreliable cellular internet connection.
** Redesigned the printed circuit board using KiCAD to add protection for the internal components, making the data logger
more resistant and accommodating to a wider range of input voltages.
** Designed an enclosure to withstand shocks and vibration during transportation.
**  Produced a construction manual, a user manual, a bill of materials, and a datasheet to document the product.
* Machine Learning Research: Soil Classification, March 2018 – June 2019
** Published a paper on a faster and more accurate process to classify soils into hydrologic groups in the journal Data as part of the
special edition Overcoming Data Scarcity in Earth Science.
** Processed soil data from USDA Natural Resources Conservation Service to extract K saturation values, percentage of sand,
silt, and clay, and the corresponding hydrologic group classifications as training data for machine learning algorithms.
** Applied K nearest neighbor, support vector machine, and random forest algorithms in MATLAB to classify soils into
hydrologic groups based on the percentages of sand, silt, and clay, and the value of saturated hydraulic conductivity.
* Internet of Things: Pet Monitoring System, March 2018 – June 2018
Designed and constructed a pet monitoring system using a GSM/GPS module, a temperature sensor, and a Raspberry Pi camera.
** Configured the GSM/GPS module with the Raspberry Pi to collect location data and send it to an InitialState streamer.
** Used the Raspberry Pi’s Camera Interface Software to create a video streaming service for the device.
** Utilized AWS IoT Core to send out tweet notifications when the temperature had reached a threshold specified by the user.
** Designed and implemented features into an IoT Button using AWS Lambda to provide easy accessibility.
Embedded System: Autonomous Robot with Amazon Alexa, September 2017 – December 2017
** Programmed, constructed, and tested an autonomous robot that could communicate through UART/SPI and navigate independently
using a 32-bit PIC32 microcontroller.
** Implemented infrared sensors on the robot to detect and follow a desired pathway.
** Utilized AWS, a Raspberry Pi, and a Wi-Fi chip to enable voice control of the robot through Amazon Alexa.
** Built a mobile application using the Apple Swift language to control the robot from a phone through the robot’s Wi-Fi chip.
** Combined the work with other teams to present the project by interacting and playing a soccer game with other robots.

Publications
======
  <ul>{% for post in site.publications %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

  
  
