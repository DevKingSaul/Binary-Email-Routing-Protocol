# New Email Format (Binary) [DRAFT CONCEPT]
#### This format will be used for the TCP Packets
|      Field      | Offset | Size |   Type   |
| --------------- | ------ | ---- | :------: |
| Username Length | 0      | 4    | UInt32BE |
| Username        | 4      | ...  |  String  |
| Domain Length   | ...    | 4    |  UInt32  |
| Domain          | ...    | ...  |  String  |

# New Email Format (Binary) [CURRENT DRAFT]
#### This format will be used for the TCP Packets. The Email Address field is the Old Email Format
|      Field      | Offset | Size |   Type   |
| --------------- | ------ | ---- | :------: |
| Email Length    | 0      | 4    | UInt32BE |
| Username        | 4      | ...  |  String  |
| Separator (@)   | ...    | 1    |  CONST   |
| Domain          | ...    | ...  |  String  |

# Old Email Format (Human-Readable / Text)
#### This format will still be used for email clients
`{username}@{domain}`


# Client TCP Header
|     Field    | Offset | Size |   Type   |
| ------------ | ------ | ---- | :------: |
| Message Type | 0      | 2    | UInt16BE |
| Extensions   | 2      | 2    | UInt16BE |

# Server TCP Header
#### Error Code is 0 for Succesful message
|     Field    | Offset | Size |   Type   |
| ------------ | ------ | ---- | :------: |
| Error Code   | 0      | 4    | UInt32BE |
