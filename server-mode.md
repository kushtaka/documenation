# Server

## Outline

Kushtaka requires an instance of `kushtakad` to be configured and running as a server in the `-server` mode.   
  
This mode has a dashboard, can send alerts, performs automatic https, facilitates the creation of tokens and facilitates the configuration of the `sensor's` along with many other administrative features.

## Steps

1. [ ] Download the executable binary for your platform
2. [ ] Set the executable bit on the binary `$ chmod +x kushtakad`
3. [ ] Run the binary passing the `-server` flag 

## Example

```text
$ wget https://github.com/kushtaka/kushtakad/releases/download/v0.1.0/kushtakad_0.1.0_linux_amd64.gz
$ gunzip kushtakad_0.1.0_linux_amd64.gz
$ chmod +x kushtakad_0.1.0_linux_amd64
$ ./kushtakad_0.1.0_linux_amd64 -server
```

