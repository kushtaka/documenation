# Overview

## Goal

Kushtaka's goal is to simplify the installation and coordination of deception techniques so that Blue Teams can protect their networks and systems through actionable signals.

## Technical

The executable is a single binary built and compiled using `Go`. This will allow for `kushtakad` to run on many different architectures. Linux, Windows, ARM would be the ideal platforms to target. All the assets are compiled into the application and this faciliates easy installation and configuration.

The datastore is `bboltdb` which is a maintained fork of Ben B. Johnson's `boltdb` project. Boltdb has many many users of the years. The database can store terabytes of data and has transactions.

## Configurator

The `kushtakad` dashboard is used to configure your Kustaka environment, create tokens and sensors, along with many other administrative tasks. When firstrunning the executable this is the default mode.

## Sensor

Sensors impersonate and emulate real life services on your network. Telnet, Ftp, Http with plans for many others. The idea is that as attackers pwn your user's machines, the network can actual act as a strategic defensive position.   
  
Because the attackers will have to move laterally and pivot to other machines/servers on the network, they must scan and probe other servers or services. It is here where the `kushtakad` executable running in `-sensor` mode can give the Blue Team a significant advantage. 

## Tokens

Tokens currently are Weblinks, Pdf or Docx files that Kushtaka generates. You place these files generated assets inside your infrastructure in places that **NO ONE** should be. When an attacker interacts with these tokens an alert is sent.























