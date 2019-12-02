# Snap

### Install

The following commands will install `snap` and `snapd`.

You then run the commands to install`kushtakad` from the `--edge` channel in `--devmode`. 

```text
$ sudo apt install snap snapd
$ sudo snap install kushtakad --edge --devmode
```

You can now see that `kushtakad` has the following services.

```text
$ sudo snap services
Service           Startup  Current  Notes
kushtakad.sensor  enabled  inactive -
kushtakad.server  enabled  active   -
$
```

### Configure Sensor

If you go to `http://localhost:8080` you will see the dashboard for the `kushtakad` server running.  
  
Once you create `sensor` on the `kushtakad` dashboard, take the `apikey` and the `host` information and run the following command.

```text
$ sudo kushtakad -apikey YOUR_API_KEY -host http://localhost:8080
```

### Disable

You can disable either of the  services with the following commands.

```text
$ sudo snap stop --disable kushtakad.sensor
$ sudo snap stop --disable kushtakad.server
```

### Enable

Similarly, you can start and enable the services with the following commands.

```text
$ sudo snap start --enable kushtakad.sensor
$ sudo snap start --enable kushtakad.server
```

