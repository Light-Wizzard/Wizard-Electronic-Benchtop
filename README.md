# Wizards Electronic Test Station (WETS)

WETS is in a single case that has many useful test equipment you can access,
using a Touch Screen, or Remotely using an Android Application, 
as such, it is an Electronic Test Station Equipment case.

WETS is a confusing acronym to use at first, but it also makes since if you want to jump in and get you feet wet in Electrons,
this one single case Test Station,
is designed to replace all the tools you normally use,
to having them all in one case.

This project currently does not have anything real to show,
it is now a startup page that explains the project that I am working,
it will have source code,
as well as links to all the Schematics,
blue prints, documents, images, videos and other electronic data,
as well as links to other projects it might work with.

The reason it is a Wizard, is because of the way the User Interface works,
it has Wizard screens that most people known about,
Programmers understand the meaning,
you have a list of things you can do,
you pick one,
for example,
you will have an option to pick a specific test equipment,
you will have a list of only Test Equipment,
and not other equipment that is not part of an Single Board Solution or SBS,
for example,
Oscilloscope,
the first box will be if you want to turn it on or maybe off if it is on,
the next Wizard screen will ask you how you want it set up,
and go through a series of settings,
all the input channels are off by default,
so you have turn them on manually,
unless you are running a test program,
that can turn equipment on and off,
as well as set it up for the task at hand,
and what Wizards help you to accomplish with as little key strokes as possible,
allowing the user to skip the Wizard at any time.
The Wizard is a pop up screen,
so it is a blocking screen,
and therefore,
you must finish with the Wizard to get back to screens under it.

From a beginner to a professional Electronics Technician or Engineer, 
you will need Electronic Test Equipment, 
and we want it all in one equipment case, 
so that is what this Project is all about.

## Index

* [List of SBS Projects](https://github.com/Light-Wizzard/Wizards-Electronic-Test-Station#List_of_SBS_Projects)
* [What is WETS](https://github.com/Light-Wizzard/Wizards-Electronic-Test-Station#What_is_WETS)
* [Test Station](https://github.com/Light-Wizzard/Wizards-Electronic-Test-Station#Test_Station)

## What is WETS

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
* Vector Signal Analyzer (VSA)
* Time Domain Reflectometer (TDR)
* Power Load Analyzer

Each item in this List can be any equipment you currently own,
and are willing to interface with, 
this means if you have for example an Oscilloscope,
you must wire up and harness to it,
this means every knob or control,
and power input, 
must have wires that can connect to the WETS system,
were WETS means getting your feet wet,
you must understand the risk of standing in water while using this equipment to stay safe,
as such, you can use any equipment that you can interface with.
This means that if you design the case for 16 channel inputs,
and you Oscilloscope only has 2, 4 or some other number,
when you set the active SBS to Oscilloscope, 
you have lights indicating which inputs are available, 
as well as which inputs are turned on.
The concept is to use Open Source Software and Hardware to fill the holes in the case with,
and every SBS is a project.

This SBS list is not set in stone,
and my concept is that you can take any equipment you currently have,
and interface it with this case,
as such, this project is more about the case,
and what projects you can use to populate it,
and you should be able to use any equipment you currently have,
and is the goal of this case,
how do you do this and make it easy to remove each SBS,
which any equipment you have that is in a case,
is considered a Single Board Solution,
this term actually means that it is contained in one removable box,
this infers that the Board itself is a box that the equipment is placed in,
this is for easy of removal, and sets the size for the equipment in the case,
proving mounting point.

The SBS cases have access to all the features you have control or monitoring over,
this includes power on/off, and all adjuster knobs,
as such, the case must have all the knobs,
so of them are push button variable knobs,
so might have more than one variable knob on its shaft,
for course and fine control,
you have push buttons for up, down, left, and right,
and function selection switch's,
and this means you to have an Active Screen,
for example a DMM, 
when it is active, all the controls that are hardwired to the interface,
most have a remote function to change that as well,
as such, the program keeps track of the position of all switch's, knobs, and controls,
for every SBS as well as other equipment in the case,
and it must have a way to indicate what controls are possible,
so lighted controls are a must, 
at least have an LED next to it,
indicating you can use this control for that SBS or Equipment.

I call other Equipment, as that of the Case itself,
for example its Power Management,
that also includes its UPS,
and you want to monitor that at all times,
and there will be other things that the Case has,
this might be options that are unique to this case,
like features you need for Automated testing of Equipment.

## Test Station

A Test Station means it has Test Equipment you have Access to,
but the Unit under test, can have Automated Testing,
this means you have all your probes setup,
this means setting up input power,
so it uses the Power Supply,
and you have test points, and each might need a different SBS,
yet you only want to use one Probe, so you have a Probe Section,
this is a patch panel of cables that can be electronically routed to the input of output of any SBS,
this allow a program to power up and down a test unit,
and using attached probes, 
it can route the signal to the right location,
and test the results for a pass or fail,
thus a technician runs the Test Program,
the Wizard tell them what probe goes where,
and what type of probe to use,
power, signal, or level probes are standard,
level probes are coaxial probes that have a known load value,
you can also calibrate your probes,
this is required to use the Oscilloscope SBS,
and a good practice to ensure you let the system know what impedance and other characteristics the cable has,
and why a Time Domain Reflectometer (TDR) is part of the list of SBS,
you can measure the length of some cables,
and find out many things about that cable with them,
so Probe calibration Wizards will walk you through connecting,
testing, calibrating, and connecting it to the unit under test.

A Test Station is not a collection of test equipment, 
it is a collection of test equipment you can access via an IO interface,
of connecting wires,
and you can apply or remove power,
and test the input and output of a unit,
as well as test all the test points on the board of the unit under test,
using a series of Wizard Screens,
that make sure you have the right probe hooked up for the current test,
and then display a pass/failure message,
as well as troubleshoot all failures.

An Automatic Test Station will still require user intervention,
the Automatic part is done in the Probe Panel,
it automatically routes the probe to the unit under test,
to the correct test equipment and sets it up for the current test,
and then deciding if that test passes or fails,
as such, Automatic means the user is told what probe goes where and when,
and when you can disconnect each probe, 
so you do not have a mess of unused probes,
and why the W in WETS is Wizard,
because a Wizard Screen will explain what probe goes where, 
and then automatically sets up that test.

Why you want a Test Station and not just a collection of Test Equipment,
is simple, 
if you have a piece of equipment that you work on,
and have schematics for it, 
you can write a C++ or a QT JavaScript program,
the two supported Qt options,
that are used to run a series of tests,
depending on the Unit Under Test (UUT), 
you have to write Wizard Screens that ask the Technician questions,
or instructs them to use test probes, and show you what point you are probing,
as well as why,
and then test the results for what you expect to find at that test point.

An Automatic Test Station Program requires the use of a known good UUT,
that means you have to have a working unit like the one you need to test,
and once you have a known good unit, 
you write a test, you can find all the test points on the board,
and known what you are looking for,
and what equipment you need,
you can write a procedure to test that point,
and know what to expect,
so you can write this test program,
and name it, save it, so you can import it,
and run it,
and you can add more test points as needed,
so the program does not need to be all encompassing,
but if you want to know if you have good board,
you will need a good board to write each test point procedure.

The Application allows you to test just a one test point,
and you can also skip tests, 
and you might want to write a test that includes a lot of component probing,
and some tests will require a lot of probing,
as well as it might need some signals from the Waveform Generator or Power Supply,
so you can write very detailed and exhaustive tests,
meaning tests that include everything you can thing of.

You have edit mode and run mode, edit mode allows you to alter the test procedure,
this allows you to make that test better,
by adding more details to the test,
or better instructions, or to alter the value of what is a pass or fail value.

A Test Station is a Machine that can be used to make an collection of equipment more useful for technicians,
than any collection of machines can possibly have any usefulness,
when it comes to repairing equipment,
and once you understand what a Test Station is,
you will never want anything else,
which is the point of this Project.

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
System RAM is 256 KB,
Retention Ram is 64 KB,
Boot Ram is 128 KB,
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

## List of SBS Projects

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
