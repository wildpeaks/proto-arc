# Arc

VRML PROTO (based on `IndexedFaceSet`) that generates part of a flat circle (e.g. for **pie charts**),
similar to [PROTO ArcLine](https://github.com/wildpeaks/proto-arcline).

	EXTERNPROTO Arc [
		exposedField  SFFloat  fromAngle
		exposedField  SFFloat  toAngle
		exposedField  SFFloat  radius
		exposedField  SFFloat  tesselation
		field         SFBool   solid
	] "proto.Arc.wrl#Arc"


-------------------------------------------------------------------------------

## Property `fromAngle`

**Start angle** (in radians).

Definition:
 - Field Type: `exposedField`
 - Data Type: `SFFloat`
 - Default Value: `0`


-------------------------------------------------------------------------------

## Property `toAngle`

**End angle** (in radians).
If `toAngle > fromAngle`, the mesh is generated **clockwise**, otherwise **anti-clockwise**.

Definition:
 - Field Type: `exposedField`
 - Data Type: `SFFloat`
 - Default Value: `6.28318`


-------------------------------------------------------------------------------

## Property `radius`

**Radius** of the circle.

Definition:
 - Field Type: `exposedField`
 - Data Type: `SFFloat`
 - Default Value: `1`


-------------------------------------------------------------------------------

## Property `tesselation`

Intermediary steps on the curve.
In short, **higher tesselation = rounder shape = more vertices**.

Definition:
 - Field Type: `exposedField`
 - Data Type: `SFFloat`
 - Default Value: `16`


-------------------------------------------------------------------------------

## Property `solid`

Like `IndexedFaceSet.solid`, specifies if the geometry is two-sided (`solid FALSE`) or one-sided (`solid TRUE`).

Definition:
 - Field Type: `field`
 - Data Type: `SFBool`
 - Default Value: `FALSE`


-------------------------------------------------------------------------------

