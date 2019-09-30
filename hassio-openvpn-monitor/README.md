# openvpn-monitor


## Summary

openvpn-monitor is a simple python program to generate html that displays the
status of an OpenVPN server, including all current connections. It uses the
OpenVPN management console. It typically runs on the same host as the OpenVPN
server, however it does not necessarily need to.

[![](https://raw.githubusercontent.com/furlongm/openvpn-monitor/gh-pages/screenshots/openvpn-monitor.png)](https://raw.githubusercontent.com/furlongm/openvpn-monitor/gh-pages/screenshots/openvpn-monitor.png)


## Configuration

### Configure OpenVPN

Add the following line to your OpenVPN server configuration to run the
management console on 127.0.0.1 port 5555:

```
management 127.0.0.1 5555
```

Refer to the OpenVPN documentation for further information on how to secure
access to the management interface.


### Configure openvpn-monitor

Copy the example configuration file `openvpn-monitor.conf.example` to the same
directory as openvpn-monitor.py.

```shell
cp openvpn-monitor.conf.example openvpn-monitor.conf

```

In this file you can set site name, add a logo, set the default map location
(latitude and longitude). If not set, the default location is New York, USA.

Once configured, navigate to `http://myipaddress/openvpn-monitor/`

Note the trailing slash, the images may not appear without it.


## License

openvpn-monitor is licensed under the GPLv3, a copy of which can be found in
the COPYING file.


## Acknowledgements

Flags are created by Matthias Slovig (flags@slovig.de) and are licensed under
Creative Commons License Deed Attribution-ShareAlike 3.0 Unported
(CC BY-SA 3.0). See http://flags.blogpotato.de/ for more details.
