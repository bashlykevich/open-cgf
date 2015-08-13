# Introduction #

As at June 2008 this project is under active development. It is currently being tested with at least one real live CDFs (SGSN/GGSNs/etc). Details of the compliance will be released once testing is complete.

If you'd like to use this in your (test) network, please do so and send any questions or feedback to feedback@3gtelcotools.com or raise an issue here. [You can download a release tarball of open-cgf from here.](http://www.3gtelcotools.com/3GPP/charging_gateway_function_cgf.html)

This server is feature complete but requires testing before it can be labelled production grade.

# TODO #

Things to do rough priority order


  * Write unit tests for encode/decode
  * Write more complex integration tests using new framework
  * Enhance test program to simulate failures/failovers
  * Exercise and debug failures/failovers
  * Rework CDR logging to make it more streamlined, simple, and faster
  * Make it optionally log in TS 32.297 CDR file format, although I'm not sure anyone uses it.

# DONE TO DATE #

  * Proper Erlang directory structure
  * Proper Erlang application, with a supervisor
  * Decoding of GTP' and all IEs from 0 up to version 2 (release 8 spec).
  * UDP daemon listener
  * Logging server which is sequence number aware
  * Listener tied to decode, tied to logging server
  * Make server reply to echo and node\_alive requests
  * Make logging server log to disk
  * Make logging multi-process
  * Make server respond to CDF (SGSN/GGSN) with data\_record\_transfer\_response periodically, which should make it very efficient. Response is tied to physical disk logging and successful file closure.
  * Auto-version fallback on version\_not\_supported messages. Configurable starting version.
  * Support for GTP' v0 20-byte header.
  * Redirects CDFs when disabling/shutting down
  * Detects and ignores duplicates as per 3GPP TS 32.295
  * Proper startup script w/ability to run as daemon and shut it down from command line
  * Syslogs (via UDP) to localhost:514. You must allow your syslog daemon to accept remote syslogs for this to work.
  * Added configuration for the syslog
  * Added the ability to run an OS command asynchronously every time a CDR file is closed.
  * Added .cdr extension to filename
  * Added logfile option
  * Fixed integration issues around sequence numbers and reuse.
  * Make TCP server work, for GTP' clients who like TCP. Sad little things.
  * Enhanced test program for TCP (and UDP)