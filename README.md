# IBM-PROJECTS

SMART WATER MANAGEMENT

1) Directly you can simulate this model by using this link : https://wokwi.com/projects/380553351208403969 
And should follow the steps provided in 3) THINGSPEAK and 4) REAL-TIME VIEWING PLATFORM which is below in this readme file


Or Otherwise to build this :

2) WOKWI:
First we should design the model which is in the image below:

![image](https://github.com/venkata9392/IBM-PROJECTS/assets/141986407/2193c47f-35f4-4330-9a23-2d64f8676c62)

First Components Needed:
a) ESP32
b) Ultrasonic Sensor
c Potentiometer
d) VCC
e) GND

![image](https://github.com/venkata9392/IBM-PROJECTS/assets/141986407/358c849c-c0f6-44d0-935b-4d30fa59c791)


Connections:

Ultrasonic Sensor Connections:
i) Connect VCC of Ultrasonic Sensor to VCC which we added.
ii) Connect GNG of Ultrasonic Sensor to GND which we added.
iii) Connect TRIG of Ultrasonic Sensor to esp:26 in ESP32.
iv) Connect ECHO of Ultrasonic Sensor to esp:25 in ESP32.

![image](https://github.com/venkata9392/IBM-PROJECTS/assets/141986407/5b568add-de6b-4b60-89dd-55e3027b6321)

Potentiometer Connections:
i) Connect VCC of Potentiometer to esp:3V3 of ESP32.
ii) Connect GND of Potentiometer to esp:GND.2 of ESP32.
iii) Connect SIG of Potentiometer to esp:3 of ESP32.

![image](https://github.com/venkata9392/IBM-PROJECTS/assets/141986407/8f2679a9-ce0a-4e7b-a4f7-3bc82b73ee7f)





Then we should use the sketch.ino file.
The diagram.json will be updated as we design the model in first step.
Then we should install needed libraries which is in libraries.txt.
We should change the CHANNEL ID and API_KEY of ThingSpeak in this code to your ThingSpeak channel's ID and API_KEY.

![image](https://github.com/venkata9392/IBM-PROJECTS/assets/141986407/752c4e3a-8039-4b0e-a937-02e3f8c6effb)


Then we can run the program .
And we can get output of the model.

![image](https://github.com/venkata9392/IBM-PROJECTS/assets/141986407/6afd29aa-053c-40e8-b7fb-43f8d777df63)


Here we get the water level output and ph value which tels whether the water is contaminated or not.

3) THINGSPEAK:
Then we want to open an account in ThingSpeak and should create a New Channel.
And Should create two fields named water level in CM and pH value.

![image](https://github.com/venkata9392/IBM-PROJECTS/assets/141986407/a238641b-b6f6-4c85-b61f-3e9da2c2834f)


We will connect the wokwi model to this ThingSpeak by using the CHANNEL ID and API_KEY of your ThingSpeak channel.
Then we want to run the Wokwi model and we will get the output data in ThingSpeak as Values and Graphs.

![image](https://github.com/venkata9392/IBM-PROJECTS/assets/141986407/26b91152-6a30-44da-8815-2260b6efc828)


4) REAL-TIME VIEWING PLATFORM:
First change the CHANNEL ID and API_KEY to your ThingSpeak channel in the index.html file ,and also use the background image which is named as Waterimage.jpg and then run the file.

![image](https://github.com/venkata9392/IBM-PROJECTS/assets/141986407/e16ee481-6592-48d1-a34a-5349a3c806d7)


Then we will see two buttons which is Water Consumption Data and Contamination Level Data.

![image](https://github.com/venkata9392/IBM-PROJECTS/assets/141986407/1a7c5d6d-a264-402b-a68c-c31d663ff309)


When we click the Water Consumption Data button then we will get the value in centimetres.

![image](https://github.com/venkata9392/IBM-PROJECTS/assets/141986407/7c614c43-e853-4f3a-bff8-8b1cc8364e55)




When we click the Consumption Level Data button then we will get the output of pH value and it will tel whether the water is contaminated or not.

![image](https://github.com/venkata9392/IBM-PROJECTS/assets/141986407/ed7ba264-9410-43ab-9fc2-444d9e357bbd)






