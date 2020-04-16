# Senior-Project
## Abstract
In this report we present our project, which resulted in the production of a handheld Bluetooth device that reports electrocardiographic information and blood oxygen measurements to a companion iOS app. Our project falls within the domains of home healthcare, personal health monitoring, embedded medical devices, and mobile health.
Pulse oximetry is useful for evaluating a patient's oxygenation status non-invasively. Two sensors and a light source are used to determine the percentage of oxygen saturation. However, any motion by the user can render the measurement unusable. Improper sensor seating, seizures, short cable tethering, or tremors, can cause inaccurate readings. The pulse oximeter is also inaccurate if the user is experiencing irregular cardiac rhythms or bradycardia - an electrocardiogram is needed to measure the heart’s electrical activity. While these medical devices are widely available, the integration of both devices for the commercial market is rare. Often these features are mixed into the smart wearable market, with biometrics tossed to the side as a selling point.
The objective of our project is to modularize and integrate the electrocardiogram and blood oxygen sensors measurements by using the MAX86150 (a bio-sensor breakout board with those elements) with a microcontroller. The MAX86150 is connected to our microcontroller through a standard I2C communication interface. This microcontroller will use samples taken from the biosensor and send them over to a connected Bluetooth device. We plan on developing an iOS application which will display the results from the microcontroller. Additionally, the app will display Bluetooth connectivity status to alert the user if there are any connection problems. Modularizing our project aims to solve the problem of maintaining signal integrity when the patient moves, and having two measurements easily readable on a smartphone.

## embedded
All necessary code to build and flash our firmware onto our handheld device

## heart_watch_companion
Xcode project necessary to build and sideload our companion app onto an iPhone

## docs
Our design document plus an infographic on how to build your own handheld ECG+SpO2 device.
