# New Email Format (Binary)
#### This format will be used for the TCP Packets
|      Field      | Offset | Size |  Type  |
| --------------- | ------ | ---- | ------ |
| Username Length | 0      | 4    | UInt32 |
| Username        | 4      | ...  | String |
| Domain Length   | ...    | 4    | UInt32 |
| Domain          | ...    | ...  | String |

# Old Email Format (Human-Readable / Text)
#### This format will still be used for email clients
`{username}@{domain}`
