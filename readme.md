# Fishing Line Experiment

## Theory

The purpose of this experiment is to determine the curvature of the earth solely
by mechanical measurement.

A neutrally buoyant fishing line *L* should form a perfectly straight
line when held under high tension in a long stretch of still water of length *l*.
If we setup each end to be a small vertical distance *x* beneath the water surface *S*,
then measure the vertical distance *x + d* of *L*'s centre-point *C* beneath *S*:

* *d* > 0 will imply convexity of *S*
* *d* < 0 will imply concavity of *S*
* *d* = 0 will imply flatness of *S*

## Concept

Suppose *l* is 250 meters. Then according to TODO *d* should be +1mm in the standard
convex earth model and -1mm in the concave earth model.

### Taking measurements

Using a ruler and a digital camera it should be possible to take a very accurate
visual measurement to within a fraction of a millimetre.
A quick proof of concept with a Samsung NV30 digicam and a standard domestic ruler
demonstrates accuracy to within about 0.25mm:

![x](./img/sample.png)
![x](./img/sample-zoom.png)

With a better camera and finer ruler an accuracy of 0.1mm may be obtainable.

### Line sag

We can use Leibniz and Bernoulli's catenary curve equation
to calculate the expected sag *a* at *C* for a given line tension, length and weight.
For example, a 250m line with tension 1000N and underwater weight of 0.5g
(250m x 0.000002kg/m) would have [an expected sag of 0.15mm](http://www.spaceagecontrol.com/calccabm.htm?F=1000&a=250&q=0.000002&g=9.81&Submit+Button=Calculate).

### Sources of error

The following possible sources of error must be taken into consideration:

* air bubbles on the line

* water currents

* water temperature

* water evaporation causing increased salinity (and hence buoyancy)

* line stretch










