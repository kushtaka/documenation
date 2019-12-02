# Linux

## Linux Snap

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

If you go to `http://localhost:8080` you will see the dashboard for the `kushtakad` server running.

