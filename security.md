# Security

Security rules for this repository. Marked blocks are maintained by Harness remediation. Text outside those blocks is left as written.


<!-- harness-remediation:sec-requests-timeout -->
### sec-requests-timeout — Set timeouts on outbound HTTP calls

Outbound requests calls in authn-service use the module-level REQUEST_TIMEOUT (connect, read) so a stalled upstream cannot hold sockets open. Pass timeout=REQUEST_TIMEOUT on every new requests call.
<!-- /harness-remediation -->
