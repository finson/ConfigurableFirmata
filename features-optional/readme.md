
#Core, Optional, and Contributed Firmata Features

Firmata is a protocol for communicating with microcontrollers from software on a host computer. The [protocol](https://github.com/firmata/protocol) can be implemented in firmware on any microcontroller architecture as well as software on any host computer software package. 

The ConfigurableFirmata fork of the repository divides the capabilities of the protocol into a number of 'features' that can be included or excluded as required.

Some of the features are considered to be
**Core**, and thus are included in the src directory. No additional work is needed to include the Core features in an executable file.  They can be excluded with simple editing of the main sketch.

Some features are identified as **Optional**, meaning that they are not as likely to be required in every sketch, but they are supported and available as part of the Firmata product.  To enable an Optional feature, you must edit the appropriate `#include` directives in the main sketch AND you must install the optional feature using the Arduino library manager applied to the appropriate zip file in the features-optional directory.

Finally, other features are identified as **Contributed**.  These are features that are not supported by the main Firmata authors.  The zip file to implement a contributed feature is placed in the features-contributed directory.  Contributed features are enabled the same way that optional features are, namely, `#include` directives and library manager installation.
