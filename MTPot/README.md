# CymmetriaResearch

MTPot is a simple open source honeypot, released under the MIT license for the use of the community.

Cymmetria Research, 2016.
http://www.cymmetria.com/

Please consider trying out the MazeRunner Community Edition, the free version of our cyber deception platform.

Written by: Itamar Sher (@itamar_sher), Dean Sysman (@DeanSysman), Imri Goldberg (@lorgandon)
Contact: research@cymmetria.com

Usage:
telnet_honeypot.py [-h] config

config - Path to a JSON config file.
Available keys:
port - REQUIRED, The port MTPot will bind to.
commands - REQUIRED, A python dict containing the commands expected to receive from the scanner (Mirai e.g.) as the keys and the responses as values.
ddos_name - REQUIRED, The name of the attack (Mirai e.g.) that will appear whenever a successful fingerprint has occured
ip - REQUIRED, The IP address MTPot will bind to.
syslog_address - OPTIONAL, Syslog IP address to send the fingerprinted IPs to.
syslog_port - OPTIONAL, Syslog PORT.
syslog_protocol - OPTIONAL, Protocol used by the syslog (TCP/UDP)


A sample config file is included (mirai_conf.json) that fingerprints the open source mirai tools released here: https://github.com/jgamblin/Mirai-Source-Code

