# Email Format
|      Field      | Offset | Size |  Type  |
| --------------- | ------ | ---- | ------ |
| Username Length | 0      | 4    | UInt32 |
| Username        | 4      | ...  | String |
| Domain Length   | ...    | 4    | UInt32 |
| Domain Name     | ...    | ...  | String |
