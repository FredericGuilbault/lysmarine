# Lysmarine - A libre nav station for Raspberrypi

> * Reliable, Coherent and Open-source  :heart:  *

<br>
Lysmarine is build with the stability of the raspbian operating system to provide an easy to use lightweight and integrated toolkit for chartplotting and sensors. As we expect this software to be used offshore by non-techy people, reliablility, simplicity and autonomy is at the core of the design.

:tada: __Contributors are welcome__ :tada: at  https://gitlab.com/FredericGuilbault/lysmarine/issues
<br>




## Download & install

Lysmarine is still in the early stage, there is no lysmarine.iso image you can just put on a SD card yet. You have to refer to the lysmarine-gen repository and expect rough edges.  



## Development guidelines

### Versioning
Versioning format of lysmarine goes like this *`major.minor-status`*. Example: `lysmarine_1.3-dev`  

Possible status are: `dev`, `rc`, `release`.<br>
When the `release` tag is used, there should be no more changes made under this version number.

### Issues
If you work on lysmarine, you should create a Issue to state your intent. So others will see what you are working on.  
If you have found an issue or just something that don't feel right. Feel free to open an issue.


### Git

 * Only merges goes in the main branch. The rest of the commits should be made in a branch. Therefor, pull request should also be made in a branch.

 * Do merges, not rebases.

 * Version numbers should be indicated as tags.  

 * Hot fix should be made in a branch named as the version it patch.

 ### Documentation

The doc for lysmarine is part of this repository and generated with http://docsify.js.org

To use it localy, First install docsify:
```
  sudo npm i docsify-cli -g
```
To serve the documentation site:
```
  docsify serve docs
```
Now you should be able to access documentation on `http://localhost:3000`
