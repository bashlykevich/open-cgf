# Introduction #

The following are based on user reports and traces, this software will require testing in your network configuration before production use.

# CDF List #

## Cisco IP Transfer Point (ITP) ##
Cisco ITPs need to log CDRs when used in SMSC-bypass configuration that delivers directly to phones or to an third-paty using [SMPP](http://en.wikipedia.org/wiki/SMPP). They have a not-terribly-well-documented GTP' interface that appears to be completely differently to the Cisco GGSN GTP' interface. It is a lot less configurable.

open-cgf has had some initial successful testing with the Cisco ITP (thanks to Ilya!). It uses GTP' v0 with a 6 byte header variant.

**Your help is needed. Please comment below or raise an [Issue](http://code.google.com/p/open-cgf/issues/list)**