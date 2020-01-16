# CoppeliaSimRemoteAPI
Template For using the remote API in CoppeliaSim/V-rep. 

This is a template project for using the remoteApi in V-rep/CoppeliaSim. 

There are two different RemoteAPI's for VREP, both work with any of the supported languages. 
This projects is a C++ VisualStudio 2017 Solution that used the default (legacy) remoteAPI.
The other remoteAPI (b0remoteAPI) has a little more functionality but is much more complicated.

The remoteAPI connects to CoppeliaSim/V-rep over the network. The IP Address is currently hard coded into the project as "127.0.0.1" on port 19997.
This should just work "out of the box" as CoppeliaSim/V-rep opens up connections on that port anyway when it starts up.

If you want to use another port or connect to a different IP Address, this can be changed in the code BUT will also require CoppeliaSim/V-rep to listen on another port. This can be done by editing the file "remoteApiConnections.txt" in the CoppeliaSim/V-rep installation directory.

The code in Source.cpp just looks for a Pioneer_p3dx in the simulation and sets motor velocities to spin the robot in circles.

This will only work if there is a scene running in CoppeliaSim/V-rep that has a Pioneer_p3dx in and the simulation already running. 

The remoteAPI does has the functionality to load/start/stop simulations; The full list of function calls can be viewed here http://www.coppeliarobotics.com/helpFiles/en/remoteApiFunctionListAlphabetical.htm

Enabling the remote API - client side http://www.coppeliarobotics.com/helpFiles/en/remoteApiClientSide.htm

Enabling the remote API - server side - http://www.coppeliarobotics.com/helpFiles/en/remoteApiServerSide.htm

Remote API modus operandi - http://www.coppeliarobotics.com/helpFiles/en/remoteApiModusOperandi.htm

Remote API constants -http://www.coppeliarobotics.com/helpFiles/en/remoteApiConstants.htm
