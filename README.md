# SmartToolStation
  
WS 2017/18 - RIOT im Internet of Things - Bachelor Project of Computer Science and Electrical Engineering 
   
# What is ToolSpace?
  
ToolSpace is a management system for monitoring and administration of a tool workspace.
The goal is to develop a system, wich can be easy installed and manage diffrent tools in a comfortable and smart way.
At the entrance of the workspace, the user sign in by NFC. To rent a tool, the user first loggs into the rental terminal, afterwards he scan the required tools.
Every tool and every user has his unigue NFC tag. 
To return the tools, the user only has to place the tool back to the tool wall.
        
![Toolspaceübersicht](images/ToolSpace_Uebersicht.jpg)

**Toolwall**
  
  - A: Tool with NFC tag (:hammer:)
  - B: Tool with NFC tag (chisel)
  - C: bold scale
  - D: gauge with NFC tag, reading device
  - E: gauge with NFC tag, reading device, electronical lock
  


    
# System Overview
   
![Planungsübersicht](images/aufbau_Toolspace.JPG)


## Sensor

For detecting the tools at the wall or for logging into the Toolstation, we use NFC tags. The RIOT Bord is connected with NFC sensors. Every information about the system will be send to the backend, where it will be handled and stored. For example the login of an already registered user looks like:

``` c
put("fe80::1ac0:ffee:1ac0:ffee","/login", testdatenNeu);
```

## Gateway

## Backend

## Frontend

# ToDo Overview
- [x] README.md erstellen
- [ ] Milestones:
  - [ ] Präsentation des Projekts
  - [ ] First Mock-Up Demo
  - [ ] Release Candidate 1
  - [ ] Final Presentation
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item
