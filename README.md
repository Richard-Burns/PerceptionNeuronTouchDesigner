# PerceptionNeuronTouchDesigner
A component for bringing Noitoms perception neuron data into TouchDesigner and auto-rigging characters.

At the moment the system is designed for any Mixamo rigs. There is currently an issue where if you bring your own character into Mixamo and it isn't already aligned correctly (you need to use their rotation tool to align) then the character comes into TouchDesigner without its alignment data. 

The current system uses the Fold DAT which is a custom C++ operator but I will replace that with a Script DAT in the next version. Please report any issues to the issues page.

#### Tested in TouchDesigner 099 2019.18580

### How to Use
1. Copy the Fold DAT dll file into your Derivative Plugins folder. This is usually found at:
C:\Users\<Username>\Documents\Derivative\Plugins
2. Drag and drop the PerceptionNeuron.tox file into your project.
3. Drag an FBX file onto the Perception Neuron components FBX Rig parameter.
#### More documentation to follow.
