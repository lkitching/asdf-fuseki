# asdf-fuseki
[Fuseki](https://jena.apache.org/documentation/fuseki2/) plugin for [asdf](https://asdf-vm.com/)

## Install
Ensure [asdf](https://asdf-vm.com/) is installed and then install the plugin with

```bash
asdf plugin add fuseki https://github.com/lkitching/asdf-fuseki.git
```

## Usage
Once installed, the plugin can be used via asdf to list and install available versions e.g.

```bash
asdf list all fuseki
asdf install fuseki 3.4.0
```

The plugin exports shims for the binaries in the fuseki package including `fuseki` and `fuseki-server`. If the asdf shims directory is
on your `PATH` these should be available:

```bash
# run fuseki server
fuseki-server
```

The plugin sets `FUSEKI_HOME` to the location of the current version specified in `.tool-versions`.