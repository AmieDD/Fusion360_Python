# Fusion360 Python Scripts
<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
[![All Contributors](https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)](#contributors-)
<!-- ALL-CONTRIBUTORS-BADGE:END -->

For you python scripts to work in Fusion 360 you have to include

![](https://github.com/AmieDD/Fusion360_Python/blob/master/python_fusion360.png)

```python
import adsk.core, adsk.fusion, adsk.cam, traceback
```
## Access Python and C++ Scripts in Fusion 360
![](/images/Autodesk%20Fusion%20360%20Scripts.png)
## Objects
Fusion 360 python API is an object oriented API exposed through a set of objects. Most of the objects have a 1-1 correspondence.

## Common Object Functionality
All objects in Fusion 360 support:

- objectType – Returns a string of the object type
- classType - A static function that returns the name of a particular class. You can combine this with objectType property above to check to see if your object reference is of a certain type.
- IsValid – Returns a Boolean(true or false, alternativitely 1 or) indicates if the object reference is valid (makes sure stuff hasn't been deleted).

## Static Functions
**Python**
```python
# Creates a new ObjectCollection
objCollection = adsk.core.ObjectCollection.create()
```

### Collections - Example DeathStarCollection
**Python**
```python
# Get exisiting sketch of a DeathStarCollection.
circles = sketch.sketchCurves.sketchCircles

# Adds a method on the DeathStarCollection to create a new deathstar circle.
circle = circles.addByCenterRadius(adsk.core.Point3D.create(0,0,0), 4)

# Get the SketchLines DeathStarCollection from an existing sketch.
lines = sketch.sketchCurves.sketchLines

# Add method to create a new line on the DeathStarCollection.
axis = lines.addByTwoPoints(adsk.core.Point3D.create(-1,-8,0), adsk.core.Point3D.create(1,-8,0))
```

### Input Objects
 Example - Lets write a script to generate the revolve of our new DeathStar Circle
**Python**

### Geometry Surface

## Contributors ✨

Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tr>
    <td align="center"><a href="http://www.amiedd.com"><img src="https://avatars3.githubusercontent.com/u/7669428?v=4" width="100px;" alt=""/><br /><sub><b>Amie DD</b></sub></a><br /><a href="https://github.com/AmieDD/Fusion360_Python/commits?author=AmieDD" title="Code">💻</a></td>
  </tr>
</table>

<!-- markdownlint-enable -->
<!-- prettier-ignore-end -->
<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
