# FreeSWITCH

This is a FreeSwitch quick test image, based on version 1.10.2-release-13-f7bdd3845a~64bit, it's not able to change any default configuration, including username, password and ports.

This image is including these users from number `1000` until `1019`, all of them are using password `1234`.

## How to run?

```
$ docker run --name freeswitch -ti --rm -p 5060:5060 -p 5066:5066 lxuancheng/freeswitch
```

## How to access the FreeSWITCH CLI (fs_cli)?

```
$ docker exec -ti freeswitch fs_cli
```

## Default Values:

* Default SIP port: `5060`
* Default WebSocket port: `5066`
* User password: `1234`

## Where are all the configurations file?

All the configuration files are in the directory `usr/share/freeswitch/conf/vanilla`.
