# dragonfly-primer

![Dragonfly](https://github.com/ladybug-tools/artwork/raw/master/icons_bugs/grasshopper_tabs/small/Dragonfly.png)

This primer provides an overview of the Dragonfly components for Grasshopper.

The Dragonfly plugin supports the creation of models following the
[dragonfly-schema](https://github.com/ladybug-tools/dragonfly-schema/wiki), which is
an abstracted means of describing building geometry built on top of the
[honeybee-grasshopper](https://docs.ladybug.tools/honeybee-primer/) plugin.
By using a fundamentally 2D representation of Building geometry, where all rooms
are assumed to be extrusions of floor plates, Dragonfly makes it easier to build
models of large buildings all of the way up to the scale of urban districts.
All Dragonfly models are translatable to Honeybee models and so all Dragonfly
models can be simulated in the same engines as Honeybee, including
[EnergyPlus](https://github.com/NREL/EnergyPlus)/[OpenStudio](https://github.com/NREL/OpenStudio)
and [Radiance](https://github.com/LBNL-ETA/Radiance).

However, Dragonfly makes it easier to create these simulation models from common 2D
formats like [GeoJSON](https://en.wikipedia.org/wiki/GeoJSON).
It also enables the connection to a wider array of simulation engines including:

* [URBANopt core SDK](https://docs.urbanopt.net/) for modeling of district thermal systems
* [DiTTo / OpenDSS](https://github.com/NREL/ditto) for sizing transformers and electrical infrastructure
* [REopt Lite](https://reopt.nrel.gov/tool) for life cycle cost optimization of photovoltaics
* [Urban Weather Generator](https://github.com/ladybug-tools/uwg) for estimation of urban heat island effects

### Installation

See the [Wiki of the lbt-grasshopper repository](https://github.com/ladybug-tools/lbt-grasshopper/wiki)
for the installation instructions for the entire Ladybug Tools Grasshopper plugin (including dragonfly-grasshopper).

### Resources

Post your questions to [Ladybug Tools forum](http://discourse.ladybug.tools) and
see the [dragonfly-grasshopper](https://github.com/ladybug-tools/dragonfly-grasshopper)
repository for source code.

Please [let us know](https://github.com/ladybug-tools/dragonfly-grasshopper/issues)
if you find any mistakes in grammar or spelling in this primer and we will gladly fix them.
