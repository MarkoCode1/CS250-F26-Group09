# TITLE

## Software Title:
Autonomous Vehicle System

## Members: 
Marko Yovanovich  
Darrick Rios  
Andrew Dominic Lumba  
Nick Pasquale  
Jamai  
Nathan Shepard

# SYSTEM DESCRIPTION

## Brief Overview of System:
The Autonomous Vehicle System is a system that provides assistance for commercial 4-wheel vehicles. The system uses sensors and cameras to detect obstacles, monitor vehicle conditions, and alert the driver, who will remain responsible for driving. 

# SOFTWARE ARCHITECTURE OVERVIEW

## Architectural diagram of all major components:
![Arch Diagram](<images/Arch Diagram.drawio.png>)


## UML Class Diagram:
--Put Info HERE--

## Description of Classes:
Vehicle: Overall physical condition of the vehicle’s health
EmergencyRead: Records the info for local and disaster feeds
User: checks if the user qualified to use the system
SensorCamera: The information gathered from sensors and cameras
PathManager: Calls for the navigation and sets and manages the route from database

## Description of Attributes:
Vehicle
state: Operational status of vehicle and emergency
mileage, engineHours, oilLife, carCPU: Maintenance Check of the vehicle
numPassenger: Number of Passengers Currently in vehicle
currSpeed: Checks current speed of the vehicle
currLat, currLong: Checks the vehicle’s current location using coordinates

EmergencyRead
LocalHazard: 
NationalHazard: 
HazardPosition: 

User
LicenseAuth: Checks if the user has valid license
VideoVerify: Checks if user watched instruction video

SensorCamera
ObjectDistance: 
isForeign: Check for foreign objects
LaneMarkLeft: 
LaneMarkRight:
numObjects: Record of foreign objects encountered

PathManager
pathPosition:
pathEnd: 

## Description of Operations:
Vehicle:
	States that the vehicle is a vehicle
	Gets and sends status of vehicle
	Gets and sends milage of vehicle
	Gets and sends Oil Life of vehicle

SensorCamera:
	Checks the stability of the sensors and cameras

User:
	Checks for authorization of user

PathManager:
	Checks the path of the vehicle
	Checks for hazards

# DEVELOPMENT PLAN AND TIMELINE

## Partitioning of tasks
At first we split into two teams to make the Architectural Diagram and the UML Diagram. Then after we finished the Architectural Diagram and got feedback, we all then started working on the UML Diagram.

## Team member responsibilities 
Nathan & Nick did the Architectural Diagram

Marko made the GitHub

Darrick, Andrew & Marko worked on the UML Diagram with Nathan and Nick joining in once the Architectural Diagram was finished.

