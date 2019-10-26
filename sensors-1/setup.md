# Setup

## Overview

The Kushtaka executable also acts as a `sensor` when you pass it the `-sensor` flag. Configurations are downloaded by the sensor from the Configurator as long as a `sensor.json` file is in the same directory as the `kushtakad` executable that you expect to run as a sensor by passing the `-sensor` flag.

## Steps

* [ ] Create a `sensor.json` file inside the directory where the `kushtakad` executable is located
* [ ] Place a json object in the file \(see examples\) that contains the following
* [ ] The `key` of the sensor that you'll find on the Configurator Dashboard
* [ ] Start `kushtakad` by passing the `-sensor` flag

## Examples

### Practical 

```text
{
	"key": "9ac35aeacfd5a951a64794c75f3Bf0bc448671ab6e62a0d71993aca98c76f545",
	"host": "http://localhost:3000"
}
```

### Descriptive 

```text
{
	"key": "THE_SENSORS_API_KEY",
	"host": "THE_URI_OF_THE_CONFIGURATOR"
}
```

### Directory Listing

```text
$ ls
kushtakad sensor.json
$
```

