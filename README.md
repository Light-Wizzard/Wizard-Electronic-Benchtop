# Wizards Electronic Test Station (WETS)

WETS is in a single case that has many useful test equipment you can access,
using a Touch Screen, or Remotely using an Android Application, 
as such, it is an Electronic Test Station Equipment case.

WETS is a confusing acronym to use at first, but it also makes sense if you want to jump in and get your feet wet in Electrons,
this one single case Test Station,
is designed to replace all the tools you normally use,
to have them all in one case, 
and fully integrated.
This project currently does not have anything real to show,
it is now a startup page that explains the project that I am working on,
it will have source code,
as well as links to all the Schematics,
blueprints, documents, images, videos, and other electronic data,
as well as links to other projects it might work with.

The reason it is a Wizard is because of the way the User Interface works,
it has Wizard screens that most people know about,
Programmers understand the meaning,
you have a list of things you can do,
you pick one,
for example,
you will have an option to pick a piece of specific test equipment,
you will have a list of only Test Equipment,
and not other equipment that is not part of a Single Board Solution or SBS,
for example,
Oscilloscope,
the first box will be if you want to turn it on or maybe off if it is on,
the next Wizard screen will ask you how you want it set up,
and go through a series of settings,
all the input channels are off by default,
so you have to turn them on manually,
unless you are running a test program,
that can turn equipment on and off,
as well as set it up for the task at hand,
and what Wizards help you to accomplish with as few keystrokes as possible,
allowing the user to skip the Wizard at any time.
The Wizard is a popup screen,
so it is a blocking screen,
and therefore,
you must finish with the Wizard to get back to screens under it.

From a beginner to a professional Electronics Technician or Engineer, 
you will need Electronic Test Equipment, 
and we want it all in one equipment case, 
so that is what this project is all about.

## Index

* [What is WETS](#What-is-WETS)
* [Test Station](#Test-Station)
* [Case](#Case)
* [MPU and MCU](#MPU-and-MCU)
* [Display](#Display)
* [List of SBS Projects](#List-of-SBS-Projects)
* [Thoughts](#Thoughts)
* [Videos](#Videos)
* [Help](#Help)

## What is WETS

A Test Station is a collection of Test Equipment that has an interface that allows a computer to route equipment probes to the probes used on the unit under test,
meaning the equipment you are working on, 
and therefore, it is not like a collection of Test Equipment that is dependent on a user routing all the cables, 
and having to manually set up the test Equipment,
it automatically sets up what routing it can, 
and sets up the equipment for the test being performed.

This project is about one Case for all the Test Equipment to fit into, 
and all the equipment functions must be Single Board Solutions (SBS) that can be upgraded.

A Function is a category like an Oscilloscope or Digital Multi Meter, and some equipment can have multiple functions in one unit,
they are called an all-in-one unit or a Multi-Unit.

The following is a list of all the Functions this case will handle:

* Oscilloscope: Mixed Signal
* Spectrum Analyzer
* Protocol Analyzer: LAN, WAN, WLAN, MAN, SAN, PAN, EPN, VPN, USB, CAN, I2C, SPI and eSPI
* Logic Analyzer
* Power Supply: Variable Isolation Transformer
* Waveform Generator: Arbitrary Waveform, Frequencies ranging as much as possible
* Frequency Counter
* LCR Meter
* Component Tester for Semiconductors
* Vector Signal Analyzer (VSA)
* Time Domain Reflectometer (TDR)
* Power Load Analyzer
* Digital Multi Meter (DMM)

Each item in this list can be any equipment you currently own,
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
and your Oscilloscope only has 2, 4, or some other number,
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
this is for ease of removal, and sets the size for the equipment in the case,
proving a mounting point.

The SBS cases have access to all the features you have control or monitoring over,
this includes power on/off, and all adjuster knobs,
as such, the case must have all the knobs,
so of them are push-button variable knobs,
so might have more than one variable knob on its shaft,
for coarse and fine control,
you have push buttons for up, down, left, and right,
and function selection switches,
and this means you to have an Active Screen,
for example a DMM, 
when it is active, all the controls that are hardwired to the interface,
most have a remote function to change that as well,
as such, the program keeps track of the position of all switches, knobs, and controls,
for every SBS as well as other equipment in the case,
and it must have a way to indicate what controls are possible,
so lighted controls are a must, 
at least have an LED next to it,
indicating you can use this control for that SBS or Equipment.

I call other Equipment, like that of the Case itself,
for example its Power Management,
that also includes its UPS,
and you want to monitor that at all times,
and there will be other things that the Case has,
these might be options that are unique to this case,
like features you need for Automated testing of Equipment.

## Test Station

A Test Station means it has Test Equipment you have access to,
but the Unit under test can have Automated Testing,
this means you have all your probes set up,
this means setting up input power,
so it uses the Power Supply,
and you have test points, and each might need a different SBS,
yet you only want to use one Probe, so you have a Probe Section,
this is a patch panel of cables that can be electronically routed to the input or output of any SBS,
this allows a program to power up and down a test unit,
and using attached probes, 
it can route the signal to the right location,
and test the results for a pass or fail,
thus a technician runs the Test Program,
the Wizard tells them what probe goes where,
and what type of probe to use,
power, signal, or level probes are standard,
level probes are coaxial probes that have a known load value,
you can also calibrate your probes,
this is required to use the Oscilloscope SBS,
and good practice to ensure you let the system know what impedance and other characteristics the cable has,
and why a Time Domain Reflectometer (TDR) is part of the list of SBS,
you can measure the length of some cables,
and find out many things about that cable with them,
so Probe calibration Wizards will walk you through connecting,
testing, calibrating and connecting it to the unit under test.

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

Why you would want a Test Station and not just a collection of Test Equipment,
is simple, 
if you have a piece of equipment that you work on,
and have schematics for it, 
you can write a C++ or a QT JavaScript program,
the two supported Qt options,
that is used to run a series of tests,
depending on the Unit Under Test (UUT), 
you have to write Wizard Screens that ask the Technician questions,
or instructs them to use test probes, and show you what point you are probing,
as well as why
and then test the results for what you expect to find at that test point.

An Automatic Test Station Program requires the use of a known good UUT,
that means you have to have a working unit like the one you need to test,
and once you have a known good unit, 
you write a test, you can find all the test points on the board,
and know what you are looking for,
and what equipment you need,
you can write a procedure to test that point,
and know what to expect,
so you can write this test program,
and name it, save it, so you can import it,
and run it,
and you can add more test points as needed,
so the program does not need to be all-encompassing,
but if you want to know if you have a good board,
you will need a good board to write each test point procedure.

The Application allows you to test just one test point,
and you can also skip tests, 
and you might want to write a test that includes a lot of component probing,
and some tests will require a lot of probing,
as well as it might need some signals from the Waveform Generator or Power Supply,
so you can write very detailed and exhaustive tests,
meaning tests that include everything you can think of.

You have edit mode and run mode, edit mode allows you to alter the test procedure,
this allows you to make that test better,
by adding more details to the test,
or better instructions, or to alter the value of what is a pass or fail value.

A Test Station is a Machine that can be used to make a collection of equipment more useful for technicians,
than any collection of machines can possibly have any usefulness,
when it comes to repairing equipment,
and once you understand what a Test Station is,
you will never want anything else,
which is the point of this Project.

## Case

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
for example, the Oscilloscope should be without display, this display would normally be on a PC,
instead, all the SBS must require a way for the PI to communicate between the SBS,
it must be able to turn it on and off, 
and the Case Front Panel must be able to provide a user interface for some controls, meaning knobs, sliders, and other switches, 
as well input and output terminals.

The case size and weight must be a factor, the Power Supply is heavy,
I want an AC and a DC power supply, the AC is limited to what a voltage converter can make given an input,
for example, in America, it is 110/120 Volts 60 Hz for a single-phase,
220/240 for two-phase,
and 330/360 for 3 Phase,
and in industrial service, you can get higher,
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
but most use the Electronic Standards for their base Country,
for example, 60 or 50 Hz,
as well as the voltage level for all 3 phases, 
for Industrial and Residential,
there are many lists like this one on Wikipedia https://en.wikipedia.org/wiki/Mains_electricity_by_country
This Power Management Function,
must be able to read all the Switch settings,
for all the SBS,
and for Power, it must be able to have a screen that actually stores the correct Country,
this screen can only be accessed after the Power comes up,
and why the switches are the only way to actually set the voltage and frequency for each of the 3 phases.
The reason you monitor the input is for brownouts or blackouts,
the system must supply a UPS,
this is built into the Power Management System,
as such, this will add its size and weight of it.

The Case will have a 10" Touchscreen or larger,
the screen space needs to be able for users to customize it,
and all these need to be saved,
this system is a Linux Machine,
I would recommend using Qt with QML and C++,
you need to have a standard that will work on any platform,
including Raspberry PI,
in case you want to use another Board,
and that needs to be a requirement,
such that the design is not set around a PI,
but still needs to be a PI alternative,
as discussed above, you want as few changes in code as possible.

## MPU and MCU

The reason I did not want to use the STM32 MPU instead of a PI,
is due to the fact I have no experience in using it,
I do not own one, so I am limited to what I do own,
or am willing to buy,
but my decision was based on Memory,
currently, the PI has 8 GB or more,
the STM32MP15
https://wiki.st.com/stm32mpu/wiki/STM32MP15_microprocessor,
has less than 1 MB,
System RAM is 256 KB,
Retention Ram is 64 KB,
Boot Ram is 128 KB,
as such, you would need to have optimized code,
and my lack of experience with programming them,
means I am more likely to use a machine with more Memory,
when I have to run applications like Web Browsers,
as well as all the Applications we need to run,
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
since all, it needs to do is check to see if it can connect to the equipment,
if it is not, 
it goes into Remote Mode,
and everywhere it needs to get data,
it gets it from a URL,
instead of connection itself,
this URL can be WiFi,
LoRa should also be an Option since it has a 10-mile range,
https://en.wikipedia.org/wiki/LoRa,
and STM32 has modules for this.
The LAN might be behind a NAT,
is so, getting access to it using the Internet,
would require you have a Business Internet Account,
this allows you to set ports that are public to everyone on the internet,
and normally require you to use a localhost web page,
to set those ports,
that page might be called "into the Danger Zone",
otherwise, you are limited to the range of your connection,
which WiFi might work up to around 1,000 feet,
maybe more with extenders,
LoRa is about 10 Miles,
and what I want,
but I will design this system to use an Optional WiFi or LoRa,
or even both at the same time, 
this allows different users to use different access methods since LoRa requires a LoRa Receiver.

## Display

The display must be able to accommodate all the SBS, 
as well as all equipment that has an Interface that you can monitor,
or control,
in the case, someone wants to use all of the Functions at one time,
and you might want to show/hide them as well,
as well as rearrange where they are,
the display must be the same for Remote use,
there should be no reason that you cannot control the SBS via this interface,
the concept is that it works on the Machine,
and that creates the internet connection to the data that is displayed,
you can write the app so it only runs in Remote mode,
and if it is not remote, 
it will log all the data to a URL,
having folders for each SBS,
making it easier to access all the units that are in the powered-on state,
and show all the units powered off,
as well as a way to toggle the states of all Equipment attached to the system,
for example, the Power Management System is not an SBS,
yet you need to monitor it, and the UPS,
in case you have a power outage.

There is no reason I cannot use Open Source/Hardware Projects to use in this System,
as long as they can be interfaced with using a PI,
which also means it might need an Arduino or STM32 MCU, 
and this should be the approach this Equipment should take.

I need to make a list of Projects this Project can support,
and that means it would have to be tested with it,
as such, there will be a category for testing.

## List of SBS Projects

Warning! You will void the warranty of any equipment you modify, 
and you will need to modify any equipment you use for a Test Station,
because it has to be able to change the settings on the equipment using a computer program.

* [Oscilloscope](#Oscilloscope)
* [Spectrum Analyzer](#Spectrum-Analyzer)
* [Protocol Analyzer](#Protocol-Analyzer)
* [Vector Network Analyzer](#Vector-Network-Analyzer)
* [Logic Analyzer](#Logic-Analyzer)
* [Waveform Generator](#Waveform-Generator)
* [Frequency Counter](#Frequency-Counter)
* [LCR Meter](#LCR-Meter)
* [Component Tester for Semiconductors](#Component-Tester-for-Semiconductors)
* [Vector Signal Analyzer](#Vector-Signal-Analyzer)
* [Time Domain Reflectometer](#Time-Domain-Reflectometer)
* [DMM](#DMM)
* [Power Load Analyzer](#Power-Load-Analyzer)
* [Power Supply](#Power-Supply)
* [Other Equipment](#Other-Equipment)

### Multiple Function

Spark Fun

* [Crowd Supply ScopeFun](https://www.sparkfun.com/products/16381)

ScopeFun: This seems to do a lot more than just an Oscilloscope

* [https://www.ScopeFun.com/](https://www.scopefun.com/)
* [https://www.opensourceimaging.org/project/scopefun/](https://www.opensourceimaging.org/project/scopefun/)
* [https://hackaday.com/2016/10/06/open-design-oscilloscope-could-be-almost-free/](https://hackaday.com/2016/10/06/open-design-oscilloscope-could-be-almost-free/)
* [Digilent Analog Discovery 2 $427](https://www.sparkfun.com/products/13929)
* [HAMlab - 160-6 10W $1,400](https://www.sparkfun.com/products/15001)

### Oscilloscope

Thunder Scope

* [https://github.com/EEVengers/ThunderScope](https://github.com/EEVengers/ThunderScope)
* [Crowd Supply](https://www.crowdsupply.com/eevengers/thunderscope)

Open Circuits

* [https://OpenCircuits.com/index.php?title=Oscilloscope](https://opencircuits.com/index.php?title=Oscilloscope)

Open Source Digital Storage Oscilloscope, 4 Ch $99

* [https://www.tindie.com/products/earth_people_technology/open-source-digital-storage-oscilloscope-4-ch/](https://www.tindie.com/products/earth_people_technology/open-source-digital-storage-oscilloscope-4-ch/)

Smart Scope

* [https://www.lab-nation.com/develop](https://www.lab-nation.com/develop)
* [https://audioxpress.com/news/SmartScope-Get-you-own-open-source-oscilloscope-](https://audioxpress.com/news/SmartScope-Get-you-own-open-source-oscilloscope-)
* [https://github.com/labnation](https://github.com/labnation)

### Spectrum Analyzer

Signal Hound

* [http://www.signalhound.eu](http://www.signalhound.eu)

21 Band Audio

* [21 Bands Spectrum Analyzer](https://oshwlab.com/trayko67/21-bands-spectrum-analyzer-buttoncontrol-ircontrol-v-1-0)

13 Band Audio

* [13 Bands Spectrum Analyzer](https://projects.digilentinc.com/mark-donners/giant-spectrum-analyzer-76b302)

### Protocol Analyzer

This might be a function of an Oscilloscope

* [TOTAL PHASE BEAGLE I2C/SPI PROTOCOL ANALYZER](https://www.microchip.com/en-us/development-tool/TTP100003)
* [http://dangerousprototypes.com/blog/2010/02/25/prototype-open-logic-sniffer-logic-analyzer-2/](http://dangerousprototypes.com/blog/2010/02/25/prototype-open-logic-sniffer-logic-analyzer-2/)

Spark Fun

* [Bus Pirate](https://www.sparkfun.com/products/12942)

### Vector Network Analyzer

Libre VNA

* [https://github.com/jankae/LibreVNA](https://github.com/jankae/LibreVNA)
* [https://hackaday.com/2021/04/22/librevna-is-a-quality-open-hardware-vector-network-analyser/](https://hackaday.com/2021/04/22/librevna-is-a-quality-open-hardware-vector-network-analyser/)

Jankae VNA 

* [https://github.com/jankae/VNA](https://github.com/jankae/VNA)

### Logic Analyzer

* [https://www.sump.org/projects/analyzer/](https://www.sump.org/projects/analyzer/)
* [https://hackaday.com/2010/07/01/open-source-logic-analyzer-software/](https://hackaday.com/2010/07/01/open-source-logic-analyzer-software/)

Spark Fun

* [8-Channel](https://www.sparkfun.com/products/18627)

### Waveform Generator

Spark Fun

* [SparkFun MiniGen - Pro Mini Signal Generator Shield $33](https://www.sparkfun.com/products/11420)
* [Frequency Generator Kit - FG085 $65](https://www.sparkfun.com/products/11394)
* [SparkFun Clock Generator Breakout - 5P49V60 (Qwiic) $30](https://www.sparkfun.com/products/15734)
* [MIKROE Waveform Click $47](https://www.sparkfun.com/products/18969)
* [MIKROE Waveform 3 Click $25](https://www.sparkfun.com/products/19285)
* [MIKROE Waveform 2 Click $45](https://www.sparkfun.com/products/19340)

### Frequency Counter

* [An Open Source Frequency Meter and clock generator](https://www.open-electronics.org/an-open-source-frequency-meter-and-clock-generator/)
* [FrequencyCounter](https://github.com/LUMERIIX/FrequencyCounter)
* [Arduino compatible frequency counter](https://pandauino.com/en/arduino-compatible-frequency-counter/)
* [open-source high-frequency pulse counter for Raspberry Pi and application to Xray transmission rate measurement](https://www.arxiv-vanity.com/papers/1911.08168/)
* [Nano Counter](https://andybrown.me.uk/2016/02/21/nanocounter/)

Frequency Counter Board

* [PCB Way](https://www.pcbway.com/project/shareproject/Arduino_RF_Frequency_Counter_with_Prescaler.html)
* [GitHub](https://github.com/imsaiguy/Frequency-Counter-Board)

### LCR Meter

* [Building an LCR Meter](https://community.element14.com/technologies/open-source-hardware/b/blog/posts/building-an-lcr-meter)
* [Low Cost High Accuracy STM32 FFT LCR Meter](https://adilmalikn.wordpress.com/2019/07/07/low-cost-high-accuracy-stm32-fft-lcr-meter/)

Spark Fun

* [Capacitance Meter DIY Kit $14](https://www.sparkfun.com/products/9485)

### Component Tester for Semiconductors

* [Component Tester - Test Almost Anything](https://www.instructables.com/Component-Tester-Test-Almost-Anything-/)
* [The Arduino UNO Transistor Tester](https://create.arduino.cc/projecthub/plouc68000/ardutester-v1-13-the-arduino-uno-transistor-tester-dbafb4)
* [Amazon Kit: D-FLIFE Multifunction Meter DIY kit, Transistor Tester, NPN PNP Diodes Triode Capacitor ESR SCR MOSFET Resistor Inductance $15](https://www.amazon.com/dp/B0952SRQP7)
* [Amazon Kit: LCR-T4 Mega328 Digital Transistor Tester Resistance Capacitance Diode Triode Capacitance Resistance ESR Meter MOS PNP NPN LCR $19](https://www.amazon.com/Mega328-Digital-Transistor-Resistance-Capacitance/dp/B07WT9VVZB)
* [Amazon Kit: Treedix GM328 Transistor Tester Frequency Tester PWM Square Wave LCR Meter Voltmeter Full Color Screen Graphics DIY Kit $22](https://www.amazon.com/Treedix-Transistor-Frequency-Voltmeter-Graphics/dp/B08B817KFL/)
* [Amazon Kit: HiLetgo LCR-T4 Multifunctional Resistor Capacitor Diode SCR Inductor Triode MOSFET Tube Meter Tester component tester kit $15](https://www.amazon.com/HiLetgo-Multifunctional-Capacitor-component-Backlight/dp/B01MYU0QI3/)

### Vector Signal Analyzer

This seems to be included in other functions

### Time Domain Reflectometer

* [Simple circuit to turn your oscilloscope into a TDR](http://dangerousprototypes.com/blog/2013/03/12/simple-circuit-to-turn-your-oscilloscope-into-a-tdr/)

### DMM

EEvBlog

* [EEVblog BM235 Multimeter](https://www.eevblog.com/product/bm235/)
* [121GW Multimeter](https://www.eevblog.com/product/121gw/)
* [EEVblog BM786 Multimeter](https://www.eevblog.com/product/eevblog-bm786-multimeter/)

Spark Fun

* [MIKROE Multimeter Click $40](https://www.sparkfun.com/products/18850)
* [Circuit Setup Energy Meter Board $38](https://www.sparkfun.com/products/16846)
* [SparkX Power Meter - ACS37800 (Qwiic) $25](https://www.sparkfun.com/products/17873)

### Power Load Analyzer

AC and DC load with Analyzer,
this puts a load on the signal being routed through it,
and can analyze that load.

Need to find a source

### Power Supply

DC
 
* Variable 0-120 Volts
* Variable 3 amp minimum at 120 volts

AC

* Variable 0-120 Volts with variable amperage
* Variable 0 to a very high voltage and amperage

Need to find a source

### Other Equipment

* LoRa
* WiFi
* Resistor Box
* Capacitor Box
* Inductor Box

## Thoughts

I am a Medically Retired US Air Force Test Station Technician,
so I know about Test Stations, I know what I want in a Test Station.

In the Air Force, a Test Station is an equipment bay that has some of the equipment I am using here,
the Unite Under Test was from the (E)F-111 Avionics, 
I specialized in Terrain Following Computer, Attack System Computer, and Communications,
but worked on many other systems as well,
as such,
I know what it takes to make a very expensive Test Station,
but now I am tasked to make as cheap of a Test Station as possible,
with it having some of the capability of an expensive one.

If you are a beginner, or a Professional, 
you want all this Equipment, 
and do not see the reason to integrate it, 
you feel you can just move cables around since the Wizard Screens in the Application,
will have you moving a probe from one point to the next,
and figure that works for you,
but a Test Station like the one I am designing here,
does a few things that you will want once you have used them,
and that is a report that certifies the unit under test, 
passes all tests.

I will work on a layout with wiring as soon as I have parts to work on,
till then, 
I will use [Blender](https://www.blender.org/) to make a [Videos](#Videos) showing all this,
and explaining it.

WETS means a Wizard Popup dialog box will ask you to move proves around for example, 
and hit continue after doing so,
the is tricky at times that you have to use more than one probe,
and why you want probes that you can attach to the unit under test,
and that means specialized probes,
and you might think that using probes by hand is a good solution,
it is in fact, 
a very bad practice, 
not only from a safety point,
the Wizard will power down the UUT, 
you are not probing a live circuit,
it knows your hand can influence your measurement,
and will not allow it,
you have to use what is known as a rig,
this can be anything that is non-conductive,
and can hold the probe firmly in place,
as such,
WETS enforces the correct procedure.

You have to program all the behavior that WETS has, 
WETS is not AI-Driven,
you have to program the UUT to power down and back up when required,
and that might mean it needs to go through a series of complicated steps,
setting up various stimuli to the UUT,
for example, if you are working on a TV,
you will want to go through all the channels,
and use various test patterns to test all pixels on the display,
and you will want to test the range of the Audio system,
so you need all the equipment to pull this off, to begin with,
and the know-how,
so it is a lot of work to write a program for a piece of equipment,
and why this design has an edit mode, 
this allows a user to create a new Job,
each job is based on a specific model of equipment you are testing,
and it allows you to do what you normally do,
which is to probe around the board and see what you find,
only now, you have written the instructions to have a Wizard ask you to do what you just did,
this is called Training if you can get an AI to write the code for you,
till then,
you have to know how to write the code, 
and that code is written in Qt C++ or Qt JavaScript,
keep in mind this JavaScript gets compiled into the program,
just like C++,
so do not choose one believing it is faster than the other,
JavaScript is C for the most part,
only it has way fewer checks it can make,
C++ has more checks,
so it is less prone to programming errors,
so you have written the code that I call a Wizard,
it in turn will be saved for the next time you work on the equipment,
but if you train it everything you did last time to fix it,
the next time you run the job,
the faster you will fix the next machine,
so it is worth the effort to write programs that will guild you through the process,
or guild others that may have never worked on this model before.

A Test Station is about saving you time if you have the equipment you Manufacture, 
and Service, meaning you have to repair it,
and you have to certify that the equipment is working as it was designed,
and that means you have to probe every possible point on the board you can,
then determine if it is a pass or fails and act accordingly.

If you are a company that has many employees,
this Test Station becomes more important,
if you have a flaw in your program,
more people using it will find those flaws faster,
and can fix them or write a report to get them fixed.

The application needs to have the capability to send reports by email, or some other means,
and you might want to print out that report as well,
and you will want to have the capability of working on the system from home on a cell phone,
in case you have to fix something in the code,
and do not need to come in to do it.

Having a PI means you have the same capabilities that the PI has, 
and with at least 8 GB of RAM,
it can multitask, 
it can write the states of all the equipment to a file,
this file format is created in the program as an array of data,
you will want to humanize it by adding names to signals, power, 
and other cables that you have running between the equipment and the UUT,
that can be used in a Network Environment,
now you can use other applications to analyze that data,
and make the results available to the Application,
making remote access to that data much easier,
but if you do not want to use the Internet,
this Test Station has an optional WiFi and LoRa system,
that allows up to 1,000 feet,
and 10-mile distances,
all from a PI.

The PI has other cards that do all the hard work,
these cards might be an Arduino or STM32 MCU,
and you can have WiFi or LoRa on those devices,
so you have many options on how the PI communicates with Test Equipment,
or how it communicates to the Unit Under Test,
and all we want to do is create a file format that we can save all the Test Data in,
these variables have names you can attach to the to make identifying them easy,
the convention for naming is something that is set in stone,
and this is a good thing,
you want to have a format naming convention that never changes,
so let me explain this better.

All Test Equipment and Units Under Test,
have a set of cables that it requires to operate,
we call these cables: Power, Input, and Output,
and we can further define the Power to a polarity, voltage, amperage, frequency, and so on,
and we have input and output power,
and we can define the Inputs and Outputs any way we need, 
as such, they describe everything that is not power,
to clarify, Power is a specific type of cable or trace on a PCB,
whereas input and output are normally terminals of some type,
for example on a Computer, you have a Video Output,
it can be High-Definition Multimedia Interface (HDMI), 
but also you might have to work with other connectors, 
like Digital Visual Interface (DVI), Video Graphics Array (VGA) (DE-15), 
Video In Video Out (VIVO) for S-Video, Composite video, and Component video, 
DisplayPort,
and even USB,
so you can see the can of worms you open up if you have to support all of these standards,
and this is when a Test Station makes more sense,
you can alter this Machine as many times as you need,
the concept is to create each set of functions you wish to support,
into a separate case,
for example, 
you will want to have Audio & Video to be in one case,
now you have room to support all standards in both,
and you have a cable that connects it to the Main Terminal,
and Terminal means it has a Monitor and Keyboard input,
and why that is important for this WETS system.

The first letter for this naming convention is the cable or trace designator,
all cables and traces only have two options, they are either an input or an output,
as such we have:

* I = Input
* O = Output

The second letter is what type of power or signal is on that cable or trace,
it can be Power, meaning it is used only to power something,
or it is a Signal,
which describes everything including the Power,
but distinguishes between what is used to power something,
from what is a signal that is used for some purpose,
this limits the options to:

* P = Power
* S = Signal

The third letter is what type of energy is on this cable or trace,

* D = Direct Current or DC
* A = Alternating Current or DC

The forth letter is what polarity it is,
we have 3 options:

* + = Positive
* - = Negative
* A = Alternating

The fifth letter is the voltage level, 
meaning the Volts, level means it can + or -,
or alternating,
this does not mean it is Alternating Current,
it means the level of this signal can be + or - at times,

* N = A positive number that represents the value, for example, 5 for 5 Volts, we already defined polarity

The sixth letter is the voltage-current,
you need to start off with the current polarity, you can have a negative polarity with a positive voltage level,
next is the current level, this is a  number, we already defined what polarity it is,

* A = A positive number that represents the current value, for example, +6A for 6 amps, +6MA for 6 milliamps, -6mA for 6 microamps, and so on.

The seventh letter is the frequency,
this can be + or -,
and you have to add the unit, like Hz, MHz, and so on

* F = Frequency, for example: +1Hz for 1 Hz

We have a template of IO:Signal-Type:Power-Type:Polarity:Voltage:Amperage:Frequency
as such, we know if this Trace or Cable is an Input or an Output,
and what type of Trace of Cable it is, Power or Signal,
and what type of Power it is, AC or DC,
and what the Voltage, Amperage, and Frequency are,
and I cannot think of what else we need to know,
it is a trace or a cable, and that means it is electricity,
if we know what the Frequency is we can calculate the wavelength,
by taking the Speed of Light and dividing that by the Frequency,
Frequency x Wavelength = Speed of Light,
but still, 
there are more properties,
and why I said this is only a starting point,
you have Capacitance, Inductance,
and Resistance, but those are all dependent on the type of measurement being taken,
as such,
you have to have two points to determine those values,
and you may not be able to accurately measure those types of components in a circuit,
yet we still need a way to define all the values for all the different measurements,
and means you have to look at every piece of equipment you have in the Test Station,
and determine all the different characteristics we need to define.

You end up with a colon (:) separated list,
and need to prefix it with a useful name that has no spaces, 
the length should never be an issue, but it cannot have a colon (:) in it.

InputPower:I:P:A:A:120:+6A:60Hz
OutputPower:O:P:D:+:60:+:0
Sensor-A:I:S:D:A:5:0
PowerGood:O:S:D:A:3:0

From here you and add more characteristics of that signal,
and not all of them need a value, but do need to have a placeholder,
and now we can read the data from the equipment,
and store it in a file using this defined format,
that can be used by applications that analyze this data.

These files tell you what you have measured inside the unit under test,
it tells you that it has an input voltage of 120 Volts at 6 Amps 60 Hz,
not hard for a computer to figure that out,
it is just a matter of what all these Signal Names mean,
and how to figure out if that is a pass or fail,
and to accomplish this we make a file that tells what these values should be,
if it is a pass it should look the same,
if it is a fail, it means something is not the same,
and it knows what is wrong at that point.

I am sure you can write a naming convention that describes everything you will need to know,
this is just a start for defining such a convention and if you can think of more,
just add an Issue and I will add it here,
so that this becomes the standard for describing all signals,
and now we have a known format for files,
so we know what the data means, 
and now we can use external applications to look at the values we have recorded,
and analyze the data for not only pass/fail,
but signs of failure.

You want to write an application to manage this naming convention,
it will need to write the application itself,
you will need to manually input the expected values,
therefore,
you need to know the Maximum and Minimum values,
but now the naming convention is too long to talk about,
and why I stopped here,
in reality, you have to define not only Electricity,
but the components you are measuring,
and you might want to put that data into another file,
such that you have values that only describe your electrical signals,
and another file that describes the measured component values,
this will make analyzing files easier,
since the two types of data are not the same,
and this method will allow you to have equipment specific naming conventions,
and allows us to specialize these file formats,
making the system very flexible.


## Videos

In Work.

I plan on making a series of videos that fully explain all aspects of the type of Test Station I am designing for the WETS System.

## Help

If you have any interest in this project, 
just make an [Issue](https://github.com/Light-Wizzard/Wizards-Electronic-Test-Station/issues),
in the subject just give as good of a short description as possible,
and I will try my best to respond to your questions.

If you have SBS links please add the SBS link: and the name of the Project,
then add the link to the Issue itself,
explaining a little about the SBS,
and I will look at the project,
and add it if I think it might work,
but will give you a response either way,
and give you a chance to respond if I have some reason not to include it,
and I must have some justification,
for example, we have an SBS that is better for this Test Station.

I am working on a [Wiki](https://github.com/Light-Wizzard/Wizards-Electronic-Test-Station/wiki).

#### End of Documents
