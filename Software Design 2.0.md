---------------------

## Software Design Specifications

---------------------

**Software Title:**

Autonomous Vehicle System

---------------------

**Members:** 

Marko Yovanovich  
Darrick Rios  
Andrew Dominic Lumba  
Nick Pasquale  
Jamai  
Nathan Shepard

---------------------

## SYSTEM DESCRIPTION

**Brief Overview of System:**

The Autonomous Vehicle System is a system that provides assistance for commercial 4-wheel vehicles. The system uses sensors and cameras to detect obstacles, monitor vehicle conditions, and alert the driver, who will remain responsible for driving. 

---------------------

## SOFTWARE ARCHITECTURE DIAGRAM 2.0

**Architectural diagram of all major components including databases:**

---------------------
this is the old database right now

![Arch Diagram](<images/Arch Diagram.drawio.png>)

---------------------

## DATA MANAGEMENT STRATEGY

---------------------

insert SQL diagram: here is the Movie Kiosk diagram as an example:
<img width="722" height="482" alt="SQL layout drawio" src="https://github.com/user-attachments/assets/df84b97f-c0e7-44f1-8718-3c65afc658cb" />

---------------------

**Tradeoff Discussion:**

SQL is generally easier to read and is more accessible.
An alternative to our data management design is to use a non-SQL language. Despite the many options in non-SQL designs such as JSON or Redis, 
these formats are still just as widely applicable as SQL, and may offer a more compact and efficient design visually.
But when all methods fundamentally fulfill the same purpose, we find the tradeoffs to be in accessibility and readability when approaching methods other than SQL. 
