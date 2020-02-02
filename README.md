# ssh2webapp
Wrapper script of Azure CLI and ssh for connecting to App Service on Linux

## Install

```sh
$ git clone git@github.com:horihiro/ssh2webapp.git
$ cd ssh2webapp
$ chmod +x ./ssh2webapp
$ ln -s $(pwd)/ssh2webapp /usr/local/bin/ssh2webapp 
```

## How to use

```sh
$ ssh2webapp -n <sitename>
```

`<sitename>`: a part of default FQDN of the app. <br>
i.e. `<sitename>.azurewebsites.net`

## Requirements
This uses Azure CLI and jq command inside.
You need to install them.

### versions

#### Azure CLI

```
$ az --version
azure-cli                         2.0.80


command-modules-nspkg              2.0.3
core                              2.0.80
nspkg                              3.0.4
telemetry                          1.0.4

Python location '/opt/az/bin/python3'
Extensions directory '/home/horihiro/.azure/cliextensions'

Python (Linux) 3.6.5 (default, Jan 13 2020, 05:03:40) 
[GCC 5.4.0 20160609]

Legal docs and information: aka.ms/AzureCliLegal
```

#### jq

```
$ jq --version
jq-1.5-1-a5b5cbe
```

