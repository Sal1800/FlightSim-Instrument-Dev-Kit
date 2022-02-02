
# FlightSim-Instrument-Dev-Kit
3D models and code to easily add detailed flight instruments to your Microsoft Flight Simulator 2020 aircraft projects.

## Getting Started
Before you begin to think about adding flight instruments, you will need to become familiar with the process of creating a third-party aircraft. The [SDK Documentation](https://docs.flightsimulator.com/html/index.htm) will be your primary source of information. 

You will also need to install at least [Blender](https://www.blender.org/download/) version 2.8 and the Blender2MSFS exporter addon appropriate for the Blender version you choose.

Download the Instrument Dev Kit files from this repository and unzip in a location near your aircraft project files. 

### Adding an instrument model to your project
From your aircraft Blender model file, select File -> Append and locate the instrument dev kit Blender file that contains the instrument you wish to add. 

The Append dialog box shows all the possible data that can be appended. Select Collections and locate the collection containing the instrument of interest. You can select multiple instruments by control-clicking to select as many as you need.



### Positioning the instruments
Now that you have the instrument collection and objects, it's not likely that they are positioned in the correct place for your panel. While you can grab and move them, there is a more precise method.

The 3D cursor will be one of the key tools to position objects precisely where you want them. Additionally, you can utilize the Item Panel to set the location by entering the X, Y & Z coordinates.

Objects in Blender are located based on their origin point. The instruments each use a root node that is positioned in the center of the instrument dial. 

