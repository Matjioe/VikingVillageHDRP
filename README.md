# VikingVillageHDRP
![Alt text](./Snapshots/VikingVillage.jpg?raw=true "Title")
This is a personal side project.
Porting Unity 5 Viking Village demo To HDRP.
Also contains Volund and Challenger characters from the Blacksmith demo converted to HDRP.
For the water I used an adaptation of https://github.com/flamacore/UnityHDRPSimpleWater

Changes made compared to the original version:
-Vegetation: Randomly added some vegetation from the HDRP template (some of the original vegetation being Terrain Details and not supported yet on HDRP).
-Ground shader: I slightly adapted the maps in order to use the HDRP layered lit material.
-VFX: For the torches, the fire was working by default with Shuriken on HDRP, but I had to use one of the provided Particle material graph sample (from the HDRP package sample) and slightly modify the graph in order to use the red channel of the albedo map as alpha.
-Lighting: Used physical units for the directional light (day) and point lights (night)
-Added Post processing volumes for rendering options, camera effects and colors, volumetrics and environment.

Bonus:
-Decals: randomly added decals from the HDRP template.
-VFX: Added VFXGraph butterflies (from the HDRP Template) on top of some bushes.
-VFX: VFXGraph dust particles (from the HDRP Template) at the center of the village and under water.
-VFX: Added volumetrics and density volumes with procedural noise (from HDRP template) in the areas close to the torches to simulate the fog accumulating around them. 
-Under water: for fun added a volume under the water overriding colors, depth of field, distortion... and added a few VFXGraph dust particles there.
-Sky: Used HDRP procedural distortion to make the clouds move
