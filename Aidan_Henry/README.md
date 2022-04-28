# Σκηνή
![image](/Aidan_Henry/Render_1.jpg)

<p align="center">
    <p align="center">Pavillion Render</p>
</p>

## Project Description
The project Σκηνή (“tent” in Greek) stems from a common ritual on the CMU campus: painting the fence. Between midnight and dawn, student organizations often paint the famous CMU fence. Sometimes more than one organization tries to do it at the same time; in the case of a standoff, tradition dictates that whoever stays by the fence longer wins the right to paint the fence. Members of organizations take turns keeping watch and often sleep by the fence in multi-day relays. We created a rest area and parasol that allows both for surveillance of the fence. Another key ritual of student organizations is also facilitated: tabling. Shade is provided in connection with the amount of sunlight parts of the pavilion receive allowing for a light but glareless habitation. 

**Contents**

- [Σκηνή.pdf](/Aidan_Henry/apsmith_hvonrint_M6 FINAL.pdf) of M6 submission
- additional [Sun_Analysis.gif](/Aidan_Henry/apsmith_hvonrint_sun-analysis.gif) and [Panel_Movement.gif](/Aidan_Henry/apsmith_hvonrint_panel-movement.gif) 
- [FCD_M6.gh](/Aidan_Henry/apsmith_hvonrint_gh.script.gh) script file
- [FCD_M6.3dm](/Aidan_Henry/apsmith_hvonrint_rhino.3dm) CAD model file
- this [Text](/Aidan_Henry/apsmith_hvonrint_README.txt) README

## Instructions for Use

This project uses a _Grasshopper_ script&mdash; which is a file that contains the algorithm to generatively design our spaceframe. You must have Rhino 7 to open the [FCD_M6.3dm](/Aidan_Henry/apsmith_hvonrint_rhino.3dm) file. The _Grasshopper_ script requires downloading the Rhino Plugin _Ladybug_ to run the daylight simulations. Once the software is correctly downloaded and the file is opened the sketch will contain a key that also details the following information. There are two input boxes in dark blue groups. The first contains the parameters for changing the size of the spaceframe and the second holds the parameters for selecting a day and time of the year to run the simulation. The light blue groups provide extra information and notes for using the rhino geometry. The yellow groups are currently hidden but when viewed they display the sun simulation.

**Dependencies**

The _Grasshopper_ script uses:
  - Ladybug

Install these dependencies and then open the [FCD_M6.gh](/Aidan_Henry/apsmith_hvonrint_gh.script.gh) file in Rhino3D.

## 3D Assets and Organization

The spaceframe was generated in _Grasshopper_ then baked into _Rhino_ space where it was organized into layers. The model was manipulated and cut using clipping planes to create orthographic drawings and renders. The images were post processed in _Adobe Illustrator_ and _Photoshop_ where materiality was added. 
