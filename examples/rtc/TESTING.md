RTC EXAMPLE
============

# Objectives
------------
This example aims to test RTC (Real-time Clock).


# Example Description
---------------------
This example demonstrates how to use the Real-Time Clock (RTC) peripheral.

The RTC enables easy time and date management and allows the user to monitor
events like a configurable alarm, second change, and calendar change.

# Test
------

## Setup
--------
Step needed to set up the example.

* Build the program and download it inside the evaluation board.
* On the computer, open and configure a terminal application (e.g. HyperTerminal
 on Microsoft Windows) with these settings:
	- 57600 bauds (for sama5d2-xplained)
	- 115200 bauds (for sama5d4-xplained)
	- 8 bits of data
	- No parity
	- 1 stop bit
	- No flow control
* Start the application.
* In the terminal window, the following text should appear (values depend on the
 board and chip used):
```
 -- RTC Example xxx --
 -- SAMxxxxx-xx
 -- Compiled: xxx xx xxxx xx:xx:xx --
 Menu :
 t - Set time
 d - Set date
 i - Set time alarm
 m - Set date alarm
 q - Quit
```

Tested with IAR and GCC (sram and ddram configurations)

In order to test this example, the process is the following:

Step | Description | Expected Result | Result
-----|-------------|-----------------|-------
Run this example | Print `[Time/Date: ` ... `[Alarm status:]` on screen | PASSED | PASSED
Press 't' | Print `Set time(hh:mm:ss):` on screen then set the time | PASSED | PASSED
Press 'd' | Print `Set date(mm/dd/yyyy):` on screen then set the date | PASSED | PASSED
Press 'i' | Print `Set time alarm(hh:mm:ss):` on screen then set the alarm time | PASSED | PASSED
Press 'm' | Print `Set date alarm(mm/dd/):` on screen then set the alarm date | PASSED | PASSED
Press 'p' | do calibration | PASSED | PASSED
Press 'q' | Print `Software Interrupt` on screen | PASSED | PASSED


# Log
------

## Current version
--------
 - v1.3

## History
--------