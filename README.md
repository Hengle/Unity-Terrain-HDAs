# Unity-Terrain-HDAs
![](Documentation/Images/Banner.jpg)


HDA's for creating Terrain in Unity with Houdini Engine\
HDAs created and tested with Houdini 19.0.498\
Assets in images from [Terrain Sample Asset Pack](https://assetstore.unity.com/packages/3d/environments/landscapes/terrain-sample-asset-pack-145808 "Terrain Sample Asset Pack") & [Unity Terrain - HDRP Demo Scene](https://assetstore.unity.com/packages/3d/environments/unity-terrain-hdrp-demo-scene-213198 "Unity Terrain - HDRP Demo Scene")



## unity_terrain_basic_example.hda
A HDA provided to as a learning guide to show you how to assign attributes for material, details and trees.


## unity_terrain_auto.hda
This HDA is designed to automate the process of assigning materials details and trees. You can define the layers in houdini and then make all the assignments in Unity.

## How to use the unity_terrain_auto.hda - in progress
Important: If you are already familiar with Houdini engine and unity this process is fairly simple. However there is an issue with HDRP that is resolved here.

Steps:

Copy the files into your otls directory "C:\Users\YourUser\Documents\houdini19.0\otls"

Place the node in houdini\
<img src="Documentation/Images/Add_Node.jpg" align="center" width="800"/>

Allow editing of contents
<p align="center">
<img src="Documentation/Images/Allow_Edit.jpg" align="center" />
</p>

Save As your new node so your changes won't modify the original
<p align="center">
<img src="Documentation/Images/Save_As.jpg" align="center" width="800"/>
</p>

Remove nodes and replace with your own terrain setup. When assigning material layers the sum of the layers must equal 1\
<img src="Documentation/Images/Remove_Nodes.jpg" align="center" width="250"/> <img src="Documentation/Images/Nodes_Deleted.jpg" align="center" width="250"/> <img src="Documentation/Images/Replace_Nodes.jpg" align="center" width="250"/>


Save Node Type

Use HDA in Unity project
![](Documentation/Images/HDA.jpg)

Assign Textures
![](Documentation/Images/Assign_Textures.jpg)

Assign Trees
![](Documentation/Images/Assign_Trees.jpg)


Assign Details
![](Documentation/Images/Assign_Details.jpg)

## IMPORTANT: Details with HDRP
The instancing property for details needs to be enabled for use with HDRP

![](Documentation/Images/HDRP_Support.jpg)
![](Documentation/Images/Edit_Details.jpg)
![](Documentation/Images/Instancing_Disabled.jpg)
![](Documentation/Images/Instancing_Enabled.jpg)