### Qos ###

This is a Linux bash script that will set up tc to limit the outgoing bandwidth for connections to the Runencoin network. It limits outbound TCP traffic with a source or destination port of 9333, but not if the destination IP is within a LAN (defined as 192.168.x.x).

This means one can have an always-on runencoind instance running, and another local runencoind/runencoin-qt instance which connects to this node and receives blocks from it.
