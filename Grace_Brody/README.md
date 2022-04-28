# Reverbrae

![Final Render 2](https://user-images.githubusercontent.com/104153711/165654317-a3f9fdc4-5d81-4ef7-92ff-b2d9b60771a8.jpg)


   <p align="center"></p>

Reverbrae is a structure on the Carnegie Mellon University cut which serves a multi use performance space. Its shape is a funnel which amplifies the sound out into the campus and improves the acoustics of the space. Reverbrae is also reminiscent of a spiral with benches that are generated from the overarching structure. The structure slopes down towards the south which provides shade at various points in the day and diffuses sunlight throughout the structure. Additionally a double layered system is used with the space frame which softens the light and creates a variety of lighting conditions throughout the day. Within the double layered system there is a series of solar panels which charge during the day and illuminate Reverbrae at night. 

**Contents**

- `.pdf` of M6 submission
- <a href="https://drive.google.com/file/d/1V1-ISXI7UBL-NjZOvCuPtkcihTg_CGj9/view?usp=sharing">Sunlight GIF</a> and <a href="https://drive.google.com/file/d/1GvlSnrJTQY0O2DFIGIWG4seEBtZRlmal/view?usp=sharing">Module Assembly GIF</a>
- <a href="https://drive.google.com/file/d/1IQOZvJTd32Hmql3mc7BvDlo_Pof-2uAt/view?usp=sharing">Grasshopper Script</a>
- <a href="https://drive.google.com/file/d/1g947DVzAWE23Nptva18PhQjSoFiyp_rT/view?usp=sharing">Rhino 7 File </a>
- this `.md` README

## Instructions for Use

This project uses a <a href="https://drive.google.com/file/d/1IQOZvJTd32Hmql3mc7BvDlo_Pof-2uAt/view?usp=sharing">Grasshopper Script</a>; which is a file that contains the algorithm to generatively design our spaceframe. You can use it in conjuction with the <a href="https://drive.google.com/file/d/1g947DVzAWE23Nptva18PhQjSoFiyp_rT/view?usp=sharing">Rhino 7 File </a> to see how to structure goes together. 

In Grasshopper, the structure uses a base curve that was generated in Rhino 7 using the "Sweep 2", "Project", and "Trim" commands. This surface is internalized in the Grasshopper file and will not need recreated. To make the script work, a <a href="https://drive.google.com/file/d/1PK4at0mnhMgRzYYU6OjgPazVxbAiFMui/view?usp=sharing">EPW File </a> for Pittsburgh's weather is needed. An input for the EPW is highlighted in the Grasshopper Script. This file contains sun path information that controls the position of the sun based on the hour of the year. The position of the sun changes the rotation of the exterior panels of the structure. The hour of the year can be changed with a slider that is highlighted in the Grasshopper Script. 

![Reverbrae Grasshopper Script Image](https://user-images.githubusercontent.com/104153711/165669413-4357d5b1-51b7-4ec6-a960-7ba6f82cbbc7.png)


To arrive at the final design, a series of edits were conducted in Rhino 7. These steps are described in the <a href="https://drive.google.com/file/d/1g947DVzAWE23Nptva18PhQjSoFiyp_rT/view?usp=sharing">Rhino 7 File </a>.

The design for the module for the structure is found in the <a href="https://drive.google.com/file/d/1g947DVzAWE23Nptva18PhQjSoFiyp_rT/view?usp=sharing">Rhino 7 File </a>. This module is derived from the original structure, but was modeled with more detail in Rhino 7. 

**Dependencies**

The <a href="https://drive.google.com/file/d/1IQOZvJTd32Hmql3mc7BvDlo_Pof-2uAt/view?usp=sharing">Grasshopper Script</a> uses:
  - Lunchbox
  - Ladybug
  - Pufferfish

Install these dependencies and then open the <a href="https://drive.google.com/file/d/1IQOZvJTd32Hmql3mc7BvDlo_Pof-2uAt/view?usp=sharing">Grasshopper Script</a> in Rhino3D.

