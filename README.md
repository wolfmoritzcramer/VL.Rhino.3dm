
# VL.Rhino.3dm

The VL.Rhino3dm library equips developers with an efficient method for integrating McNeel's Rhinoceros 3D files into their VL projects. This plugin simplifies the process of importing Rhinoceros 3D files, enabling direct access to their geometry, material properties, and user-defined strings within the VL programming environment.

By natively supporting Rhinoceros files in VL, developers can avoid the cumbersome process of tweaking 3D model export settings, a common obstacle in alternative workflows. Additionally, the library enhances functionality with a BIM-like workflow, permitting the attachment of custom information to each model object. This metadata enrichment not only facilitates innovative collaboration methods but also optimizes the tool's application for specific tasks. Importantly, it empowers developers to filter and locate specific objects within VL, leveraging the organizational capabilities inherent to Rhinoceros for structuring model data efficiently.



Try it with vvvv/VL, the visual live-programming environment for .NET

Download: http://visualprogramming.net

McNeel's Rhinoceros3d
https://www.rhino3d.com/

Supported by:

Jan Henrik Hansen Architects, Studio Brüll and the vvvv Community
## Usage / Installation
In order to use this library with VL you have to install the nuget that is available via nuget.org. For information on how to use nugets with VL, see Managing Nugets in the VL documentation. As described there you go to the commandline and then type:
```bash
nuget install VL.Rhino.3dm
```
 https://www.nuget.org/packages/VL.Rhino.3dm

## Course

You can find a 3h long recorded session with an in depth explanation and project examples at 

https://thenodeinstitute.org/courses/ss24-vvvv-integrating-rhino-3d-with-vvvv/


### Versions
Tested with vvvv gamma (VL) 6.5 and Rhino 8.6 (Rhino Files are downward compatible)


### Geometry
Points, Curves, Surfaces, Breps, SubDs, Meshes are currently supported.
You have to activate at least one time the shaded view inside Rhino, the displayed rendermesh quality is the quality you get inside vvvv.

### Materials
Works best with PBR Materials, Texture Mapping is (due to a bug in Rhino) currently only supported with files done in Rhino7 (saving as Rhino7 from Rhino8 does not help) 
As there are differences in material workflows, the materials are only an approximation but fit quite well in most cases.
It is easy to replace certain materials with your own vvvv made ones.

### UserStrings
UserStrings for objects are supported and can enhance your workflow perfectly. 

### Lights
Directional, Point and SpotLights are supported

### Blocks
Blocks contained in the file are supported and rendered as instances as well in vvvv.



