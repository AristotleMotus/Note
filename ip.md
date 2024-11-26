## Classes

| Class         | Leading bits | Size of *network number* bit field | Size of *rest* bit field | Number of networks  | Addresses per network  | Total addresses in class | Start address   | End address     | Default [subnet mask](https://en.m.wikipedia.org/wiki/Subnet_mask) in [dot-decimal notation](https://en.m.wikipedia.org/wiki/Dot-decimal_notation) | [CIDR notation](https://en.m.wikipedia.org/wiki/CIDR_notation) |
|---------------|--------------|------------------------------------|--------------------------|---------------------|-------------------------|--------------------------|-----------------|-----------------|----------------------------------------------------------------------------------------------------------------------|----------------------------|
| Class A       | 0            | 8                                  | 24                       | 128 (2^7)           | 16,777,216 (2^24)       | 2,147,483,648 (2^31)     | *0.0.0.0*       | *127.255.255.255* | *255.0.0.0*                                                                                                          | */8*                       |
| Class B       | 10           | 16                                 | 16                       | 16,384 (2^14)       | 65,536 (2^16)           | 1,073,741,824 (2^30)     | *128.0.0.0*     | *191.255.255.255* | *255.255.0.0*                                                                                                        | */16*                      |
| Class C       | 110          | 24                                 | 8                        | 2,097,152 (2^21)    | 256 (2^8)               | 536,870,912 (2^29)       | *192.0.0.0*     | *223.255.255.255* | *255.255.255.0*                                                                                                      | */24*                      |
| Class D       | 1110         | Not defined                        | Not defined              | Not defined         | Not defined             | 268,435,456 (2^28)       | *224.0.0.0*     | *239.255.255.255* | Not defined                                                                                                           | */4*                       |
| Class E       | 1111         | Not defined                        | Not defined              | Not defined         | Not defined             | 268,435,456 (2^28)       | *240.0.0.0*     | *255.255.255.255* | Not defined                                                                                                           | Not defined                |

---

## Bit-wise representation

In the following bit-wise representation:

- *n* indicates a bit used for the network ID.
- *H* indicates a bit used for the host ID.
- *X* indicates a bit without a specified purpose.

### Class A
