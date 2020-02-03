# DataDrivenDriving

## Abstract

This system aims to monitor the driving behavior of drivers by using OBD II device, which is
used in this project. It is an adapter where the data is read from the car’s Engine Control Unit
(ECU) and is transmitted via Bluetooth upon pairing. The results will be provided to the user
to improve their driving skills. It uses OBD-II protocol and an Android app as the device of
mediation. The analysis is performed offline and results will be shown on the app. This app
will provide benefit to car owners as well, as they will be able monitor the driving behaviors
of their drivers.


## Description of the Project

The rapid increase of vehicle usage has led to many concerns not only for the drivers but also
to the owners of the car. If the car owner can be made aware about drivers abnormal driving
behaviors, then it will be helpful for owners to get to know about their drivers driving behavior
and it would help them to take decision whether to let them continue as their driver or not.

This project uses On-board Diagnostics (OBD II) device and its protocols and an Android app
as the device of mediation. The OBD device is plugged into the car and communicates with
car’s ECU. This project consists of an application named Data Driven Driving (D_Cube) which
is connected with OBD-II device using Bluetooth. After successful connection with Bluetooth,
when the user presses the option of Start Live Data at the start of the trip, the live readings are
being received from OBD device till the end of the trip until the user presses the option Stop
Live Data. Driver’s current trip report will be generated after every trip using the data collected
during that trip which will tell how well the driver drove the car. The driver can also create
PDF of that report by simply clicking on the PDF button. The app also has options of Daily,
Weekly, and Monthly reports.


## Benefits

For Drivers
* Current report will help them to identify unusual behavior.
* Self-evaluation of the driver itself e.g.: how good the driver is.
* The driver will be able to improve his driving skills through current report generated
after the trip ends.

For Owners

* Through this owner will be able to make decision whether to keep the current driver or
not.
* Monitoring the driving behavior of drivers through the report generated after every trip
and notifying them for unusual driving behavior.




## Interface Preview 

<p align="center">
  <img src="https://github.com/Sameer18-Dev/DataDrivenDriving/blob/master/Assets/Animation.gif" width="300"/>
  </p>
  Driver Module
  <p align="center">
  <img src="https://github.com/Sameer18-Dev/DataDrivenDriving/blob/master/Assets/Page1.PNG" width="300"/>
  <img src="https://github.com/Sameer18-Dev/DataDrivenDriving/blob/master/Assets/Page2.PNG" width="300"/>
  </p>
  Owner Module
  <p align="center">
  <img src="https://github.com/Sameer18-Dev/DataDrivenDriving/blob/master/Assets/Page3.PNG" width="450"/>
  </p>


## Tools and Technologies ##
- Android Studio 3.3+
- AES Encryption
- NodeJS Server
- OBD Java API
- RESTful API
- Firebase
- SQLite

## Tested On ##

* Samsung Galaxy Note 2
* Samsung Galaxy Alpha
* Samsung Galaxy Prime
* Samsung Galaxy S6
* Samsung A10s
* xiaomi mi a2



## Dependencies


``` 
dependencies {
...
    compile 'com.android.support.constraint:constraint-layout:1.1.3'
    compile 'com.google.firebase:firebase-database:16.0.1'
    compile 'com.github.PhilJay:MPAndroidChart:v3.1.0'
    compile 'com.android.support:appcompat-v7:22.1.1'
    compile fileTree(dir: 'libs', include: ['*.jar'])
    compile 'com.android.support:cardview-v7:22.1.1'
    compile 'com.github.pires:obd-java-api:1.0-RC16'
    compile 'com.squareup.retrofit:retrofit:1.9.0'
    compile 'com.android.support:design:22.2.1' 
    provided 'org.roboguice:roboblender:3.+'
    compile 'org.roboguice:roboguice:3.+'
    compile 'net.gotev:uploadservice:2.1'
    compile 'com.itextpdf:itextg:5.5.10'
}
```
