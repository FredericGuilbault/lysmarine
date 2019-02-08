# LysMarine
Linux OS for Marine navigation and sensors.

#### Download & install
Lysmarine is still in the early stage, there is no lysmarine.iso image you can just put on a SD card yet. Until then, you have to refer to the [lysmarine-gen](https://gitlab.com/FredericGuilbault/lysmarine-gen) repository and expect rough edges.  

# Project structure
Lysmarine is made of different repostiores.

## The main lysmarine repo contain.
[lysmarine](https://gitlab.com/FredericGuilbault/lysmarine)
- Project page.
- Documentation.
- The Lysmarine Noob image.

## The lysmarine-gen repo is the building script.
[lysmarine-gen](https://gitlab.com/FredericGuilbault/lysmarine-gen)
*This is where the magic append* !
  It's a fork of the [pi-gen](https://github.com/RPi-Distro/pi-gen) repo used to build [Rasbian](https://www.raspberrypi.org/downloads/raspbian/).
  It have been adapted to the needs of lysmarine to create the NOOB install image.
  > Users do not need to build lysmarine, lysmarine images are available for each versions in the main lysmarine repository

## The tuktuk-chart-plotter repository.
  [tuktuk-chart-plotter](https://gitlab.com/FredericGuilbault/tuktuk-chart-plotter)
  Lysmarine have his own fork of [tuktuk-chart-plotter](https://github.com/vokkim/tuktuk-chart-plotter).
  It add some features and pre-configured settings to it.

# Documentation
The documentation of the project can be found [here.](doc/README.md)

## Contributors
Frederic Guilbault is the founder and the principal maintainer of the project.
*Contributors are welcome. (In fact, I feel a bit alone here ;) )*
