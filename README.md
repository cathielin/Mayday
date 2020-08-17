# Mayday
Given coordinates and a runway length, mayday prints a list of airports and runways long enough that are closest to the current location. The information is stored in 2 text files from the Federal Vaiation Administration. The 2 files list 19,700 facilities and over 23,000 runways. Mayday prints the 10 closest airports, (their name, code, and distance from given location) and all their runways of sufficient length.

Current position and minimum runway length are taken from the command line when the program is run.

Written in C++11

NOTE: The code for this project has NOT been uploaded to GitHub publicly, as it was done for my data structures class. This was done to avoid future students from using my code as a violation of academic code conduct.

## Implementation
The program uses two user-defined objects, Facility and Runway objects, that are stored in STL vectors. These objects are sorted using the STL sort algorithm and a function object.

## End Lessons / Notes
Demonstrates an understanding of 
<ul>
  <li>OOP concepts: writing code centered around user-defined objects</li>
  <li>Reading and processing select information from text files</li>
  <li>Sorting data stored in vectors</li>
  
  ## Example
  Position: (38.6954, -121.5910) with a minimum landing length of 6000 ft
  AIRPORT       SMF  SACRAMENTO INTL                                      0.0 NM <br>
  Runway: 16L/34R  length: 8605 ft <br>
  Runway: 16R/34L  length: 8598 ft <br>
AIRPORT       MCC  MC CLELLAN AIRFIELD                                  9.1 NM <br>
  Runway: 16/34    length: 10599 ft <br>
AIRPORT       DWA  YOLO COUNTY                                         14.3 NM <br>
  Runway: 16/34    length: 6000 ft <br>
AIRPORT       MHR  SACRAMENTO MATHER                                   16.1 NM <br>
  Runway: 04L/22R  length: 6038 ft <br>
  Runway: 04R/22L  length: 11301 ft <br>
AIRPORT       LHM  LINCOLN RGNL/KARL HARDER FIELD                      17.0 NM <br>
  Runway: 15/33    length: 6001 ft <br>
AIRPORT       MYV  YUBA COUNTY                                         24.2 NM <br>
  Runway: 14/32    length: 6006 ft <br>
AIRPORT       BAB  BEALE AFB                                           27.4 NM <br>
  Runway: 15/33    length: 12001 ft <br>
AIRPORT       SUU  TRAVIS AFB                                          30.2 NM <br>
  Runway: 03L/21R  length: 11001 ft <br>
  Runway: 03R/21L  length: 10995 ft <br>
AIRPORT       OVE  OROVILLE MUNI                                       47.6 NM <br>
  Runway: 02/20    length: 6020 ft <br>
AIRPORT       SCK  STOCKTON METROPOLITAN                               50.9 NM <br>
  Runway: 11L/29R  length: 10650 ft
