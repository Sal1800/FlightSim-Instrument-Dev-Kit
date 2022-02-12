
# FlightSim-Instrument-Dev-Kit
3D models and code to easily add detailed flight instruments to your Microsoft Flight Simulator 2020 aircraft projects.

## Getting Started
Before you begin to think about adding flight instruments, you will need to become familiar with the process of creating a third-party aircraft. The [SDK Documentation](https://docs.flightsimulator.com/html/index.htm) will be your primary source of information. 

You will also need to install at least [Blender](https://www.blender.org/download/) version 2.8 and the Blender2MSFS exporter addon appropriate for the Blender version you choose.

Download the Instrument Dev Kit files from this repository and unzip in a location near your aircraft project files. 

### Current Status
This is a work in progress. The Six-Pack instruments are ready to use in your projects. Make sure to read the documentation. Other instruments are still being developed. You can use the models but there may be more work needed.

### Adding an instrument model to your project
From your aircraft Blender model file, select File -> Append and locate the instrument dev kit Blender file that contains the instrument you wish to add. 

The Append dialog box shows all the possible data that can be appended. Select Collections and locate the collection containing the instrument of interest. You can select multiple instruments by control-clicking to select as many as you need.


### Positioning the instruments
Now that you have the instrument collection and objects, it's not likely that they are positioned in the correct place for your panel. While you can grab and move them, there is a more precise method.

The 3D cursor will be one of the key tools to position objects precisely where you want them. To move the Cursor effectively, use Shift S to open the Snap context menu. "Cursor to Selected" and "Cursor to Active" will snap the 3D cursor to the current object. This works in Object mode or Edit mode. 

The instruments in this kit each use a root node that is positioned in the center of the instrument dial. To move the instrument and all of it's child objects, select only the root object and use the Shift S -> "Selected to Cursor" command to snap the instrument to the cursor location. 


### Add the Behavior Code to your Model XML
Copy the included behavior code into your interior model XML file in the <Behaviors> section. This is all that is needed to activate the animations and knob mouse rects.

### Customizing
Most of the instruments are fairly standard across many aircraft types, so they can be used as is. Some, like the airspeed indicator will not be suitable for all types and will require some modification to handle the scale and reference speeds of the particular aircraft you are modeling. See the documentation section for details on how to draw gauge faces and calibrate the animations. 

### Troubleshooting
If the Package build process fails, the most likely reason will be a misconfiguration of the behavior XML code. Ensure that all XML tags have a closing tag. There are some online XML validation tools that may help to pinpoint exactly where the error may lie. 

