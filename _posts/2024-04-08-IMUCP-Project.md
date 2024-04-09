---
layout: post
title: "International Multidisciplinary Urban Capstone Project"
subtitle: "Modifying MATSim to model traffic in Pune"
background: '/img/posts/IMUCP/IMUCP_background.png'
---

## Contribution

Developed a custom classes to incorporate MATSim simulation to effectively analyze Pune's Traffic Network

The modifications involve:

- Importing CSV file and Parsing the data

- Modifying XML files to include fields with custom fare information

- Modifying MATSim source code to improve efficiency

[Current working in progress codes can be viwed here](https://github.com/woom221/matsim-pune-india){:target="_blank"}

Implemented a tool for effective data gathering using Google Distances API

- Developed a simple data gathering tool using Google Distances API

- Durations of travel and routes can be tested and gathered. 

- Can be easily modified to gather different information that API supports

[The baseline code can be viewed here](https://github.com/woom221/google-directions-api/tree/main){:target="_blank"}

## Technical Tools utilized

Java, JDOM, MATSim, Python, Google Distances API

### About IMUCP

International Multidisciplinary Urban Capstone Project (IMUCP) is a year-long capstone project conducted by final-year students at the University of Toronto. In this project, students are placed in multidisciplinary teams (i.e., our team consisted of students from Civil Engineering, Architecture, and Urban Studies) and matched with community partners that bring existing urban challenges that they would like the students to consult on.

This time around, IMUCP is making history by taking urban challenges from a different country - India, hence the title international. It's the first time the project is reaching beyond Canada to tackle issues in another part of the world. This shows a big step forward for IMUCP, as it now aims to address global urban problems.

[More about MUCP/IMUCP can be viewed here](https://schoolofcities.utoronto.ca/learning-sofc/mucp/){:target="_blank"}

### About Project

Being the second largest city in the province of Maharashtra, Pune is currently facing urban challenges with air quality deterioration. Pune Municipal Corporation has requested the University of Toronto to seek a solution to resolve the issue. After a thorough investigation, the primary culprit behind the pollution emerged as inefficient traffic networks leading to heavy congestion. In response to PMC's request, a tool capable of simulating and analyzing various traffic scenarios using real road data was deemed necessary.

One of the major problems we faced during the project was the lack of simulation data. I developed a quick data-gathering tool using Google Distances API that can effectively simulate the travel scenario between different locations, facilitating more accurate analyses. Another obstacle that we faced was the limitations of the existing software. The current metro system in Pune operates with fixed costs which vary by the stations. Such functionality is not implemented by MATSim software. For the naive and simple approach, I chose to modify the XML document which is used for simulation modeling directly to resolve this issue. However, this approach presented a potential problem of excessive RAM usage, particularly with a large dataset comprising 7,744 station entries already consuming 6GB of RAM. I am trying to modify the source code associated with evaluation functions directly to improve efficiency to avoid this issue.


### Code Examples

The code used for modifying XML is shown below: 

<img src="\img\posts\IMUCP\IMUCP_edit_config.png">

<img src="\img\posts\IMUCP\IMUCP_edit_config_two.png">

The code used for data generation is shown below:

<img src="\img\posts\IMUCP\IMUCP_google_distances.png">

<img src="\img\posts\IMUCP\IMUCP_google_distances_two.png">