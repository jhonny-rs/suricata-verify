## NFSv2 STATFS Parser Test

This test validates the correct parsing of the NFSv2 `STATFS` procedure.

- **`nfsv2.pcap`**: A pcap containing one NFSv2 `STATFS` packet.
- **`test.yaml`**: Checks that one `nfs` event is logged with `nfs.version: 2` and `nfs.procedure: STATFS`.
- **`test.rules`**: A rule that matches on `nfs.version: 2` and `nfs.procedure: statfs` to confirm the detection engine can use the parsed fields.