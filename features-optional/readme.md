
#Firmata Features - Core and Optional

Firmata is a protocol for communicating with microcontrollers from software on a host computer. The [protocol](https://github.com/firmata/protocol) can be implemented in firmware on any microcontroller architecture as well as software on any host computer software package. 

The ConfigurableFirmata fork of the repository divides the capabilities of the protocol into a number of 'features' that can be included or excluded as required.

Some of the features are considered to be **Core**, and thus are included in the src directory. No additional work is needed to include the Core features in an executable file.  They can be excluded with simple editing of the main sketch.

Some features are identified as **Optional**, meaning that they are not as likely to be required in every sketch, but they are fully supported and available as part of the Firmata product.  To enable an Optional feature in your program, you must:

1. Edit the appropriate `#include` directives in the main sketch 
2. AND you must install the optional feature using the Arduino library manager. The feature sources are all delivered as part of the Firmata download and are located in the ConfigurableFirmata/features-optional directory. Using the library manager menu item "Include library -> Add .ZIP library", navigate to the features-optional directory and select the folder for the feature you want and click open.  The feature will be installed in the sketch's library directory.
