# Introduction #

This page tells you how to use the test client included in the package. The test client is still under development but includes UDP and TCP tests.


# Details #

Run an erlang shell ` erl `

To perform a little test use:
`test_udp:simple_test({{65,23,156,214},3386},{{65,23,156,215}, 3386})`

The local source address and port e.g. _{{65,23,156,214},3386}_  and CGF (open-cgf) server IP address and port e.g. _{{65,23,156,215}, 3386})_ need to be adjusted for your specific site.