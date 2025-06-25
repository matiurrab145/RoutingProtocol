# RoutingProtocol
## LEACH

The LEACH (Low-energy adaptive clustering hierarchy) is a hierachical adhoc routing protocol for Wireless Sensor Networks. 
The code in this repository is an implementation of it for the [INET Framework](https://inet.omnetpp.org) of the [OMNeT++](https://omnetpp.org) simulator.


<figure>
    ![LEACH-stages-new](https://github.com/user-attachments/assets/15d8e7a8-a90f-4d19-9c46-3a1c7152d9eb)
</figure>

Follow the below steps to run the simulation.

1. Prerequisites 

2. Install OMNeT++, INET Framework -

3. Run models


## 1. Prerequisites

These models have been tested on the following versions of INET and OMNeT++.

- OMNeT++ version 5.6.2

- INET Framework version 4.2.5


## 2. Install and Build

Follow the following procedure to install and build the models.

1. Install and build [OMNeT++](https://omnetpp.org)

2. Create a new workspace in the OMNeT++ IDE

3. Install and build the [INET Framework](https://inet.omnetpp.org) in the created workspace

4. Copy the `LEACHnode` and `leach` directories present in the `node` and `routing` directories respectively to the `node` and `routing` directories in the your installed INET project.

5. Import the `LEACH3` project into the workspace via `Existing project into Workspace` option. Link it with INET using `properties > project references` and ticking on the `inet` option.

6. Rebuild INET and LEACH3  projects


## 3. Running Models

- Use the *omnetpp.ini* files provided in the LEACH3 directory to run the simulation

- Important parameters are referenced via comments within the *omnetpp.ini* file.

## File structure

<figure>
    ![file-structure](https://github.com/user-attachments/assets/03811b36-ccd1-48df-96c1-746884bafd2a)


</figure>

The simulations consists of 3 layers organized by their directories;

- Simulation components - `<workspace_home>/LEACH3`

- Node intermediary layer - `<workspace_home>/inet4/src/inet/node/LEACHnode`

- Node routing logic layer - `<workspace_home>/inet4/src/inet/routing/leach`

