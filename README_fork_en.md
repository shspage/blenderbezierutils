# Changes from [the original repository](https://github.com/Shriinivas/blenderbezierutils)

by [@shspage](https://github.com/shspage)


## ver.0.9.96+  -  2020.12.27

(Merge remote-tracking branch 'upstream/master')

----

## ver.0.9.95+2  -  2020.12.17

### Added "Vertex" mode to handle snap function
_Vertex mode_ has been added to each of the pie menu items ("Selected Ends" and "Move Paths").
In Vertex mode, the destination of the endpoint is not the (mathematical) closest point on the Bezier curve, but the closest location of the vertex when the curve is converted to a mesh.

 (The position of the vertices is determined based on the resolution of the curve (BezierCurve> Shape> Resolution Preview).)

----

## ver.0.9.95+1  -  2020.12.16

### Added handle snap function
Moves the endpoint of the selected _Bezier curve_ on the nearest point on the _Bezier curve_. At that time, adjust the angle of the handle to the tangent line at the destination.

After selecting the endpoint in object mode (with the Flexi Edit Bezier tool), press **Shift + S** to display the pie menu. Select one of the following.

- **Selected Ends** : Moves the selected endpoints.

- **Move Paths** : Moves the endpoints and applies the movement to the entire path. If both endpoints are moved, the average of the moves is applied to the other points.

### Supports Retina display
The default values such as font size and line width are multiplied by `bpy.context.preferences.system.ui_scale`.

(I'm not sure if this is the correct way to deal with this problem. I would appreciate it if you could point out.)

----
