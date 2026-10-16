# User Class

## Unit Test

Authorize(): bool

Unit Test: Tests whether the user is authorized to operate the autonomous vehicle by verifying that they have a valid driver's license and have completed the instructional video. 

Input: LicenseAuth: bool (true if license is valid, false otherwise
Input: VideoVerify: bool (true if user watched video, false otherwise)
Output: Return bool (true if both input are true, false otherwise) 


User u  
u.LicenseAuth = true  
u.VideoVerify = false  

if(u.Authorize() == false)  
	Return PASS  
else  
	Return FALSE
 

## Integration Test

Type here 

## Sysytem Test 

The goal of the User System Test is to verify that the that the driver of the vehicle is a authorized user of the vehicle. For this to happen a user of the vehicle will input their email and password via the Vehicle App or Vehicle screen itself. If the person in the vehicle is not a user the system will prompt them to make a account via a link to the Autonomous Vehicle System Website. The user will have to input their email, name, password, age, and drivers license information for them to successfully make a account. After the user is fully signed it and the they are a authorized user, they will be able to successfully drive the vehicle.

---

# PathManager Class

## Unit Test

Pathmanager p

int lat = 35

int long = 42

int hazlat = 0

int hazlong= 0

p.PathPosition = [lat,long]

p.HazardPosition = [hazlat, long]


if( p.isValidPath == True)
	
	return PASS

else
	
	return FAIL
 

## Integration Test

IsValidPath ( PathPosition <int, int>, HazardPosition<int, int>) : 

Integration test : test that the object returns a valid path to the vehicle object or states that the path is not possible given the hazard position.
- input: PathEnd : <int, int> (target gps location)
- input: PathPosition : <int, int> <current gps location>
- output: Return bool (true if valid path exists, false otherwise)

## System Test 

To start the Path Manager will first look at the Vehicle class. The Vehicle class will grab its information from the Sensors and Cameras Class to help pinpoint object around the Vehicle. Specifically the Sensors and Camera will be able to tell how far a object is away from the vehicle, and how many object their are. Its also able to read road lines to make sure that the vehicle is able to stay within it. Our Vehicle class will also be able to grab GPS data form the cloud so the vehicle class knows the road is a road. After the vehicle grabs the data from the sensors and camera its going to work hand in hand with our path manger system which is able to grab the location of the car via Longitude and Latitude and determine the pathing. The path manger will also determine whether there are any hazards in the way of the cars destination. If everything goes smoothly and as intended the vehicle should be able to drive by itself to the desired location with out any issues or incidents. 

---------------------
