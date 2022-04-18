# Godot Basic Function
Some godot basics useful (in my opinions) functions
----
```gdscript
# Map from a range to new one
func map_range(t, min1, max1, min2, max2):
	return lerp(min2, max2, inverse_lerp(min1, max1, t))
 
# Calculate distance usually round (circle), this function make it ellipse
# Imaging circle in 3D perpective (orthorgraphic)
func ellipse_distance(p1:Vector2, p2:Vector2, f:Vector2):
	return sqrt(pow((p1.x-p2.x)/f.x, 2) + pow((p1.y-p2.y)/f.y, 2))
```
