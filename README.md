
![Logo](rhino3dmicon.png)

# VL.Rhino.3dm

The VL.Rhino3dm library equips developers with an efficient method for integrating McNeel's Rhinoceros 3D files into their VL projects. This plugin simplifies the process of importing Rhinoceros 3D files, enabling direct access to their geometry, material properties, and user-defined strings within the VL programming environment.

By natively supporting Rhinoceros files in VL, developers can avoid the cumbersome process of tweaking 3D model export settings, a common obstacle in alternative workflows. Additionally, the library enhances functionality with a BIM-like workflow, permitting the attachment of custom information/properties to each model object. This metadata enrichment not only facilitates innovative collaboration methods but also optimizes the tool's application for specific tasks. Importantly, it empowers developers to filter and locate specific objects within VL, leveraging the organizational capabilities inherent to Rhinoceros for structuring model data efficiently.


Try it with vvvv/VL, the visual live-programming environment for .NET<br>
vvvv/VL: http://visualprogramming.net<br>
McNeel's Rhinoceros3d
https://www.rhino3d.com/

<br>
## Support the Development of VL.Rhino.3dm

VL.Rhino.3dm is an independent open-source project that I maintain in my free time.  
If this library is useful in your work, please consider supporting its ongoing development.

Your contribution directly helps to maintain the codebase, fix bugs, improve documentation, and build new features.

### 🧾 For companies and professional users  
You can make a voluntary contribution via Stripe (supports invoices & VAT ID):

👉 **[Support via Stripe](https://donate.stripe.com/5kQcN51VOgXd14m9VigIo00)**

### ☕ For individuals and community supporters  
A lighter, more casual way to support the project:

👉 **[Support on Ko-fi](https://ko-fi.com/wmccc)**

Thank you for helping keep the project alive!
<br><br>
## Usage / Installation
In order to use this library with VL you have to install the nuget that is available via nuget.org. For information on how to use nugets with VL, see Managing Nugets in the VL documentation. As described there you go to the commandline and then type:
```bash
nuget install VL.Rhino.3dm
```
 https://www.nuget.org/packages/VL.Rhino.3dm

## Course

You can find a 3h long recorded session with an in depth explanation and project examples at 

https://thenodeinstitute.org/courses/ss24-vvvv-integrating-rhino-3d-with-vvvv/

---
### Versions
Tested with vvvv gamma (VL) 6.6 and Rhino3dm 8.9 (Rhino Files are downward compatible)


### Geometry
Points, Curves, Surfaces, Breps, SubDs, Meshes are currently supported.
You have to activate at least one time the shaded view inside Rhino, the displayed rendermesh quality is the quality you get inside vvvv.

### Materials
Works best with PBR Materials, Texture Mapping is supported.
As there are differences in material workflows, the materials are only an approximation but fit quite well in most cases.
It is easy to replace certain materials with your own vvvv made ones as you get a material dictionary for easy access.

### UserStrings
UserStrings for objects are supported and can enhance your workflow perfectly by giving your 3D objects properties you can use in vvvv.

### Lights
Directional, Point and SpotLights are supported but still WIP

### Blocks
Blocks contained in the file are supported and rendered resource friendly as instances as well in vvvv.

<br><br>
#### Supported by:

Studio Brüll<br>
Jan Henrik Hansen Architects<br>
...and of course the vvvv Community


