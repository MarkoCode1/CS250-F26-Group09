---------------------

## Test Cases

---------------------

# User Class

## Unit Test

Type here 

## Integration Test

Type here 

## Sysytem Test 

Type here 

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

Type here 

---------------------
