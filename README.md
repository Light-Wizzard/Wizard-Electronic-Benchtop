# Wizard Electronic Benchtop

From a beginner to a professional Electronics Technician or Engineer, you will need Electronic Test Equipment, and we want it all in one equpiment case, 
so that is what this Project is all about.

This project is about one Case for all the Test Equipment to fit into

All equipment functions must be Single Board Solutions (SBS) that can be upgraded.

The following is a list of all the Functions this case will handle:

* Oscilloscope: Mixed Signal
* Spectrum Analyzer
* Protocol Analyzer: WAN, LAN, PAN, and Wireless Networks, USB, CAN, I2C, SPI and eSPI
* Logic Analyzer
* Power Supply: Variable Isolation Transformer
* Waveform Generator: Arbitrary Waveform, Frequencies ranging as much as possible
* Frequency Counter
* LCR Meter
* Component Tester for Semiconductors
* Vector Signal Analyzer
* Time Domain Reflectometer
* Power Load Analyzer

This SBS list is not set in stone.

The case must be able to hold all these Single Board Solutions (SBS),
and the layout must have the Power Supply on the bottom, 
and you must ensure it has RF shielding, so it does not interfere with other SBS,
this is the same for all SBS.

This project will use the latest and greatest Raspberry PI, with the most Memory, 
this can be a PI Alternative,
as such, I will only say PI, but that means any Alternative that will work,
it needs to be able to communicate with all the SBS,
this might be done through another board,
like an Arduino or Alternative, like an STM32,
so I might say Arduino, but that means any Alternative that works,
as well as an STM32 MCU,
as such, these SBS must be able to have many types of cards that support it,
and that might mean you end up with a few different types of IO cards to communicate with.
The Main Computer Board, as mentioned above, can be any, 
but keep in mind each might require a different set of applications to support it,
so staying with PI and alternatives is the safest way to ensure the code does not require a lot of changes,
it is used to run the display for all the SBS, 
for example, the Oscilloscope should be a without display, this display would normally be on a PC,
instead, all the SBS must require a way for the PI to communicate between the SBS,
it must be able to turn it on and off, 
and the Case Front Panel must be able to provided a user interface for some controls, meaning knobs, sliders, and other switches, 
as well input and output terminals.

The case size and weight must be a factor, the Power Supply is heavy,
I want an AC and a DC power supply, the AC is limited to what a voltage converter can make given an input,
for example, in America it is 110/120 Volts 60 Hz for single phase,
220/240 for two phase,
and 330/360 for 3 Phase,
and in industrial service you can get higher,
but this needs to work in any Country, 
and it must have a Smart Input Detection Circuit,
so it will continuously monitor the input channels, 
and a program will monitor this feature in real-time,
and everything should be in real-time,
why I have to say it, is to make it clear you can set the time intervals for updates,
as such, this case must take into account all countries around the world, 
and to make this safe, 
you want to make a kit that will attach to the case,
the case should have only Single, Dual, and 3 Phase inputs, 
with a switch for base Country,
there are a lot of Countries, 
but most use the Electronic Standards of its base Country,
for example, 60 or 50 Hz,
as well as the voltage level for all 3 phases, 
for Industrial and Residential,
there are many list like this one on Wikipedia https://en.wikipedia.org/wiki/Mains_electricity_by_country
This Power Management Function,
must be able to read all the Switch settings,
for all the SPS,
and for Power, it must be able to have a screen that actually stores the correct Country,
this screen can only be accessed after the Power comes up,
and why the switches are the only way to actually set the voltage and frequency for each of the 3 phases.
The reason you monitor the input is for brownouts, or blackouts,
the system must supply a UPS,
this is built into the Power Management System,
as such, this will add the size and weight of it.

The Case will have a 10" Touchscreen or larger,
the screen space needs to be able for users to customize it,
and all these need to be save,
this system is a Linux Machine,
I would recommend using Qt with QML and C++,
you need to have a standard that will work on any platform,
including Raspberry PI,
in case you want to use another Board,
and that needs to be requirement,
such that the design is not set around a PI,
but still needs to be a PI alternative,
as discussed above, you want as few changes in code as possible.

The reason I did not want to use the STM32 MPU instead of a PI,
is due to the fact I have no experience in using it,
I do not own one, so I am limited to what I do own,
or am willing to buy,
but my decision was based on Memory,
currently the PI has 8 GB or more,
the STM32MP15
https://wiki.st.com/stm32mpu/wiki/STM32MP15_microprocessor,
has less than a MB,
System RAM is 256KB,
Retention Ram is 64KB,
Boot Ram is 128KB,
as such, you would need to have optimized code,
and why I did not include it as an option,
but I do plan one using STM32 MCU,
https://www.st.com/en/microcontrollers-microprocessors/stm32-32-bit-arm-cortex-mcus.html.

This system should have an Android App to go with it,
my idea is to make it the app,
so we do not have two programs,
using Qt QML with C++,
this is possible,
the way it works is by making one variable to track if it is a Remote connection,
this can be written into the app,
since all it needs to do is check to see if it can connect to the equipment,
if it is not, 
it goes into Remote Mode,
and everywhere it needs to get data,
it gets it from a URL,
instead of connection itself,
this URL can be WiFi,
LoRa should also be an Option since it has a 10 mile range,
https://en.wikipedia.org/wiki/LoRa,
and STM32 has modules for this.
The LAN might be behind a NAT,
is so, getting access to it using the Internet,
would require you have a Business Internet Account,
this allows you to set ports that are public to everyone on the internet,
and normally require you to use a local host web page,
to set those ports,
that page might be called "into the Danger Zone",
otherwise you are limited to the range of your connection,
which WiFi might work up to around a 1,000 feet,
maybe more with extenders,
LoRa is about 10 Miles,
and what I want,
but I will design this system to use an Optional WiFi or LoRa,
or even both at the same time, 
this allows different users to use different access methods sine LoRa requires a LoRa Receiver.

The display must be able to accommodate all the SBS, 
as well as all equipment that has an Interface that you can monitor,
or control,
in the case someone wants to use all of all the Functions at one time,
and you might want to show/hide them as well,
as well as rearrange where they are,
the display must be the same the same for Remote use,
there should be no reason that you cannot control the SBS via this interface,
the concept is that it works on the Machine,
and that creates the internet connection to the data that is displayed,
you can write the app so it only runs in Remote mode,
and if it is not remote, 
it will log all the data to a URL,
having folders for each SBS,
making it easier to access all the units that are in the powered on state,
and show all the unites powered off,
as well as way to toggle the states of all Equipment attached to the system,
for example the Power Management System is not an SBS,
yet you need to monitor it, and the UPS,
in case you have a power outage.

There is no reason I cannot use Open Source/Hardware Projects to use in this System,
as long as they can be interfaced with using a PI,
which also means it might need an Arduino or STM32 MCU, 
and this should be the approach this Equipment should take.

I need to make a list of Projects this Project can support,
and that means it would have to be tested with it,
as such, there will be a category for tested.

## List_of_SBS_Projects

### Oscilloscope: Mixed Signal

### Spectrum Analyzer

### Protocol Analyzer

### Logic Analyzer

### Power Supply

### Waveform Generator

### Frequency Counter

### LCR Meter

### Component Tester for Semiconductors

### Vector Signal Analyzer

### Time Domain Reflectometer

### Power Load Analyzer

#### End of Documents
