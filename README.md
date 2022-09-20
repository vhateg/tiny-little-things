# tiny-little-things
Tiny Little Things is an open-source IoT framework that strives to make developing and integrating IoT solutions easier for tinkerers.

## Why does this exist?
Due to the complexity of existing IoT frameworks, most beginner tinkerers would avoid this area or develop their own uncompatible solutions. But, by providing easy to use and understand standards and example implementations, the concepts of IoT and of smart homes can be opened to more people.

## What platform will this run on?
The target platform of this project is ESP32, but options for ESP8266 and possibly other IoT chips will be provided.

## How does it work?
TLT is composed of two main parts: smart devices that host their own HTTP servers, basically offering a HTML device interface and a REST API and client applications that combine said pages into a seamless app. There is a third pillar, a home server, that will allow both appless access (i.e. not using the native apps) and remote access and also smart features such as scenarios.

## More technicalities
Each TLT device will host a HTML page that features device-specific controls and buttons. Said controls can be also accessed via an API, for more intelligent applications, such as being controlled by a home assistant.
This approach makes everything easier for a few reasons:
* each smart device has its own page, with controls. This makes devices independent and easily controllable from any internet capable device.
* as they are basic servers, any new user in the network can easily discover the devices and control them, making guest control much easier. Of course, devices can be password protected, so access can be controlled.
* this offers a very flexible platform, as the HTTP page can be customized to the maker's liking, so any sort of feature can be implemented.

## Non-tinkerer users?
Because the products are ready-for-use as soon as the program is flashed, there is a minimal setup needed. Each device will feature an eazy to understand startup interface at the first boot, or when a reset button is pressed. After this easy setup, everything is ready to go. New 
