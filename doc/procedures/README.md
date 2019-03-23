# Install

## Install lysmarine from the NOOBS image
Lysmarine is still in the early stage, there is no lysmarine.iso image you can just put on a SD card yet. Until then, you have to refer to the lysmarine-gen repository and expect rough edges.

## Build Lysmarine From source code
```
git clone https://gitlab.com/lysmarine/lysmarine-gen.git
cd lysmarine-gen
sudo CLEAN=1 ./build.sh
```
Then you can find the NOOBS at location `work/xxx-lysmarine/export-noobs/`


## Run the documentation website

The doc for lysmarine is generated with http://docsify.js.org

To use it locally, First install docsify:
```
  sudo npm i docsify-cli -g
```
Init
```
docsify -l true  init ./

```


To serve the documentation site:
```
  docsify serve doc
```
Now you should be able to access documentation on `http://localhost:3000`
