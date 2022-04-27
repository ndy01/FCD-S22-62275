**Responsive Architecture**

Project completed for the spring 2022 run of the Fundamentals of Computational Design course taught at CMU. Explorations focused on responsiveness, performance and fabrication; we designed a space frame system with panelized components of varying materiality (opacity and tint) which could be determined based on solar radiation analysis. As demonstrated in the example project, this system can be applied to all kinds of forms, including organic ones.

The files contain one possible rendition of a pavilion using the system and a custom form we designed.

**Contents**

- [Grasshopper script](https://drive.google.com/file/d/1gHD-AdS2vbgAWeS_t9_XWexK7cgxgyCU/view?usp=sharing) - generates the space frame and panelization
- [Rhino file](https://drive.google.com/file/d/1AGwYfzpOjLsHerYscWlUozqMDaiD-0ep/view?usp=sharing) - contains example project geometries, as well as the final result generated from Grasshopper script.
- [Example EPW file containing weather information](https://drive.google.com/file/d/1_jE3WKN9-4UvzYelehn3FGsGfpIPM6NZ/view?usp=sharing) - use this when running the script on the demo Rhino file
- Additional assets - [HDRI derived from Google Maps](https://drive.google.com/file/d/1_jE3WKN9-4UvzYelehn3FGsGfpIPM6NZ/view?usp=sharing); 3D buildings of CFA and Hunt Library courtesy of SketchUp Warehouse

**Instructions/3D Assets &amp; Organization**

The Grasshopper script works by taking in a base form (as surface or polysurface), and applying panelization to it, so as to create a space frame and panes. The first portion of the script runs a radiation analysis simulation using the Ladybug plugin for Grasshopper, which requires the use of an .EPW file containing weather information. The second portion of the script is focused on creating the geometries. In order to use the script, you will need both a base geometry and a weather file.

**Parameters to change**

- Input brep - this is your base geometry! The overall form of the structure, which you want the responsive system to span across. (Even if it is a mesh, you will want to put it through Step 1, so that the model is panelized accordingly. This is important because both the space frame and the panels are based on the mesh faces and subdivision method.)
- Internalize the mesh, and set it to be &quot;base geometry&quot; for the simulation.
- Surrounding buildings (mesh) - Usually in radiation analysis we will have surrounding buildings and context which cast shadows and affect the daylighting conditions. Add them here so they are accounted for in the simulation; use a mesh-to-brep component if necessary to convert your NURBS geometry into a mesh.
- Frame thickness - determines distance between the layers which comprise the space frame.
- Pipe thickness - determines thickness of the pipes which form the space frame. If your geometry is smaller, you will need thinner pipes.

**Script dependencies and other software**

The Grasshopper script uses the following plugins:

- Pufferfish | ver: 3.0.0.0
- Weaverbird | ver: 0.9.0.1
- Kangaroo2 Components | ver: 2.5.3

It also uses multipipe (a subd) which is only available in Rhino 7 and above. For rendering, the planting also made use of Lands Design.

**References and acknowledgements**

The design of the project looked towards precedent studies which employed methods related to responsive and sustainable architecture, such as the [2009 Serpentine Pavilion from SANAA](https://www.serpentinegalleries.org/whats-on/serpentine-gallery-pavilion-2009-kazuyo-sejima-ryue-nishizawa-sanaa-0/) and [the &quot;Articulated Cloud&quot; facade system at the Pittsburgh Children&#39;s Museum](https://iibec.org/acoustics-with-kinetic-facades/).

Original 3D models for context buildings ([CMU College of Fine Arts](https://3dwarehouse.sketchup.com/model/e3c90ce951d482b897d1514a353839e/Carnegie-Mellon-College-of-Fine-Arts?hl=en) and [Hunt Library](https://3dwarehouse.sketchup.com/model/b77d183d6b44aaf7f50c99f478904ece/Hunt-Library-Carnegie-Mellon-University)) came from SketchUp warehouse, and were modeled by &quot;Nick D&quot;.
