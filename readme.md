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

Suppose *l* is 250 meters. Then *d* should be
[+1.226mm in the standard convex earth model](http://dizzib.github.io/earth/curve-calc/index.html?d0=0.25&h0=0.001226&unit=metric)
and -1.226mm in the concave earth model.

### Measuring line depth

Using a ruler and a digital camera it should be possible to take a precise
visual measurement to within a fraction of a millimetre.
A quick proof of concept with a cheap Samsung NV30 digicam and a standard domestic ruler
demonstrates accuracy to within about 0.25mm:

![x](./img/sample.png)
![x](./img/sample-zoom.png)

With a [USB endoscope](https://duckduckgo.com/?q=usb+endoscope&ia=videos)
and a [100 micron ruler](http://www.tedpella.com/tools_html/Micro-Tool-Measurement.htm)
we should be able to measure to the nearest 0.1mm.

### Line sag

We can use Leibniz and Bernoulli's catenary curve equation
to calculate the expected sag at *C* for a given line tension, length and weight.
For example, a 250m line with tension 1000N and underwater weight of 0.5g
(250m x 0.000002kg/m) would have [an expected sag of 0.15mm](http://www.spaceagecontrol.com/calccabm.htm?F=1000&a=250&q=0.000002&g=9.81&Submit+Button=Calculate).

### Sources of error

The following possible sources of error must be taken into consideration:

#### Water currents

The force *f* required to vertically displace *C* a small distance *y* is derived as
follows, using [small angle approximation](https://en.wikipedia.org/wiki/Small-angle_approximation):

    sin(theta) = (2y / l) = tan(theta) = (f / T)

    f = 2Ty / l

where *theta* is the angle subtended by the straight and displaced lines and
*T* is the tension.
So taking *l* = 250m, *T* = 1000N and *y* = 0.1mm gives *f* = 0.0008N,
showing that even a tiny net force can displace the line.
Therefore it is very important to eliminate all convection currents in the water.

#### Water temperature

Water density varies with temperature, maxing out at 4°C.
So a neutrally buoyant line in water at 16.0°C will tend to sink in water at 16.1°C.

#### Water evaporation

If a saline solution is used to achieve neutral buoyancy, water evaporation may cause
the salinity (and hence buoyancy) to increase over time.

#### Line stretch

Any line will stretch under tension and reduce its total mass underwater.
The amount of stretch is determined by its
[Young's modulus ](https://en.wikipedia.org/wiki/Young's_modulus)
and any reduction in its diameter is determined by its
[Poisson ratio](https://en.wikipedia.org/wiki/Poisson's_ratio#Width_change)

#### Air bubbles on the line
