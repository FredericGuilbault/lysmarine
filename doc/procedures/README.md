# Install lysmarine

## With NOOBS
Lysmarine is still in the early stage, there is no lysmarine.iso image you can just put on a SD card yet. Until then, you have to refer to the lysmarine-gen repository and expect rough edges.

## From source code
TODO, meanwhile plz refer to :
[lysmarine-gen](https://gitlab.com/lysmarine/lysmarine-gen)


# Install the documentation

The doc for lysmarine is generated with http://docsify.js.org

To use it localy, First install docsify:
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
