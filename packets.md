# New Email Format (Binary) [DRAFT CONCEPT]
#### This format will be used for the TCP Packets
|      Field      | Offset | Size |  Type  |
| --------------- | ------ | ---- | ------ |
| Username Length | 0      | 4    | UInt32 |
| Username        | 4      | ...  | String |
| Domain Length   | ...    | 4    | UInt32 |
| Domain          | ...    | ...  | String |

# New Email Format (Binary) [CURRENT DRAFT]
#### This format will be used for the TCP Packets. The Email Address field is the Old Email Format
|      Field      | Offset | Size |  Type  |
| --------------- | ------ | ---- | ------ |
| Email Length    | 0      | 4    | UInt32 |
| Email Address   | 4      | ...  | String |

# Old Email Format (Human-Readable / Text)
#### This format will still be used for email clients
`{username}@{domain}`
