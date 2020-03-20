Changelog
=========

v4.7
====

-   Add -v version output

-   Improved statistic reporting on exit

-   Timeouts can be set for connections based on if TCP connections are present
    or not

-   better exit codes

-   targets can now set a range of ports to bind to

-   fixed DNS resolver for static builds

-   better p2p connection rate to some symmetric NAT’s

-   fixed provisioning file reading if without a final carriage return

-   target logs connecting IP address on connection

-   base64 password to long crash fixed

v4.6
====

-   Latching Restrict IP address mode (set restrict IP to 255.255.255.255)

-   Better IP restriction error reporting.

-   Fix exit message and timeout when cannot bind to a port

-   bug fixes

-   typo fix

v4.5
====

-   Return codes are retuned on exit

-   Better error handling of port already in use condition.

-   Performance enhancements

-   Copyright update.

v4.4
====

-   Multiple P2P connections to one service connection fix.

-   Service only logs in once at startup.

v4.3
====

-   vReporting.

-   Copyright update.

v4.2
====

-   Zero window starvation fix.

-   Spelling error fix

-   CPU utilization reduction

-   NATPMP windows corner case fix

v4.1
====

-   Ping time control for P2P links optimized and fixed

-   `!!` return codes always returned correctly

-   `!!` return codes have numeric values added

-   Suppress output now works for `-nc`

v4.0
====

-   Change the binary names to "connectd".

-   Ping time control for P2P links

-   Command line configuration via base64 blobs (`-e` option)

-   Nat Checker (`-nat`)

-   Bug fixes
