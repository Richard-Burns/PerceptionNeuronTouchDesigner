# Perception Neuron TouchDesigner Component
A component for bringing Noitoms perception neuron data into TouchDesigner and auto-rigging characters.

At the moment the system is designed for any Mixamo rigs. There is currently an issue where if you bring your own character into Mixamo and it isn't already aligned correctly (you need to use their rotation tool to align) then the character comes into TouchDesigner without its alignment data. 

The current system uses the Fold DAT which is a custom C++ operator but I will replace that with a Script DAT in the next version. Please report any issues to the issues page.

#### Tested in TouchDesigner 099 2019.18580

### How to Use
1. Extract the Fold DAT zip file and copy the Fold DAT dll file into your Derivative Plugins folder. This is usually found at:
C:\Users\<Username>\Documents\Derivative\Plugins
2. Drag and drop the PerceptionNeuron.tox file into your project.
3. Drag an FBX file onto the Perception Neuron components FBX Rig parameter.

### Axis Neuron Settings

#### General 
- Set Port to 7001

#### Output Format
- Frequency reducing should b 1
- Rotation should be XYZ
- Displacement should be checked, reference unchecked
- Quaternion should be Sensor global
- Acceleration should be Sensor local
- Angular velocity should be Sensor local

#### Broadcasting
- Tcp/Udp should be set to UDP
- BVH should be enabled
- Format should be String
- ServerPort should be 7001
- ClientPort should be 7002
- Use old header should be unchecked