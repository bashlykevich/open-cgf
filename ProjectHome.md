This project provides a 3GPP-compliant Charging Gateway Function (CGF) as a sink for SGSN/GGSN/etc streamed CDRs on the 3GPP Ga/Gz interface. Refer 3GPP 32.295. These are common data elements of GSM/UMTS mobile telephone networks. This is part of the toolkit developed by [3G Telco Tools](http://www.3gtelcotools.com).

![http://www.3gtelcotools.com/images/GSM%20UMTS%20Core%20Network%20v00.01.gif](http://www.3gtelcotools.com/images/GSM%20UMTS%20Core%20Network%20v00.01.gif)

The CDRs are streamed over the [GTP'](http://en.wikipedia.org/wiki/GTP%27) (GTP-prime) protocol, a subset of the main [GPRS Tunnelling Protocol](http://en.wikipedia.org/wiki/GPRS_Tunnelling_Protocol) (GTP) protocol used between the SGSN and GGSN.

open-cgf implements all the features of 32.295 although not all SGSN/GGSNs implement, and therefore exercise, these features. It is not yet clear if any CDFs (GGSNs/SGSNs/etc) implement the special sequence number/duplicate-avoidance features described in this standard.

**See the [Wiki current project status](http://code.google.com/p/open-cgf/wiki/CurrentStatus)**

| **[open-cdf release 0.13 is available for download from here](http://www.3gtelcotools.com/3GPP/charging_gateway_function_cgf.html)** | **Updated June 3rd 2008** |
|:-------------------------------------------------------------------------------------------------------------------------------------|:--------------------------|

Contributions and feedback, including traces from your network, are welcome and appreciated.
Send them to feedback@3gtelcotools.com

