# IP Addresses in Relation to the OSI Model

- Not hardcoded
- Can be mapped to any MAC address that we specify

## Structure of an IP Address

- 32bit Binary Address (each IP address will have a mix of 32 ones and zeros)
- Divided into four sections known as "Octets"
- Octets each have eight bits
- Each Octet has a possible value of 0 - 255 (256 possibilities)

## Calculate an IP Address with binary values

- Take binary representation of IP Address and add each section by it's place in the table below if it's "on" (value of 1)

<b>IP Address: 192.160.1.1</b>

| 1   | 1  | 0  | 0  | 0 | 0 | 0 | 0 |
|-----|----|----|----|---|---|---|---|
| 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |

- 128 + 64 = 192

| 1   | 0  | 1  | 0  | 0 | 0 | 0 | 0 |
|-----|----|----|----|---|---|---|---|
| 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |

- 128 + 32 = 60

| 0   | 0  | 0  | 0  | 0 | 0 | 0 | 1 |
|-----|----|----|----|---|---|---|---|
| 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |

- 1 = 1

| 0   | 0  | 0  | 0  | 0 | 0 | 0 | 1 |
|-----|----|----|----|---|---|---|---|
| 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |

- 1 = 1

# Calculate binary values from IP Address

- Start from left most Octet in the IP Address
- Start from left most column in IP Address table (128)
- If IP Address is larger than that value at 1 to that column and subtract that columns value from the Octets value
- Continue until you hit 0
- Move right one Octect
- Repeat

<b>IP Address: 192.60.1.1</b>

| 1   | 0  | 0  | 0  | 0 | 0 | 0 | 0 |
|-----|----|----|----|---|---|---|---|
| 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |

192 - 128 = 64

| 1   | 1  | 0  | 0  | 0 | 0 | 0 | 0 |
|-----|----|----|----|---|---|---|---|
| 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |

64 - 64 = 0

Our first Octet is now represented as <b>11000000</b> in Binary.