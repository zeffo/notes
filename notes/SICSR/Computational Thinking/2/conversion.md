# Conversion

## Decimal to Binary

1) Divide the number by 2 and note down remainder. 
2) Repeat till you obtain 0.
3) Concatenate the remainders and reverse to obtain the binary number.

**Example**:
Our number is 389.

| Number | Remainder |
| ------ | --------- |
| 389    | 1         |
| 194    | 0         |
| 97     | 1         |
| 48     | 0         |
| 24     | 0         |
| 12     | 0         |
| 6      | 0         |
| 3      | 1         |
| 1      | 1         |
| 0      | 0         |

Therefore 389 in binary is:
**110000101**

## Binary to Decimal

We'll do the inverse of the [Decimal to Binary](conversion.md#Decimal%20to%20Binary) process.

1) Read the number from right to left.
2) Start with p = 1 and number = 0. For every subsequent digit, `p = p * 2`
3) Multiply p with the digit and add it to number: `number += digit * p`

**Example**:
For the number 110000101:
`1*1 + 0*2 + 1*4 + 0*8 + 0*16 + 0*32 + 0*64 + 1*128 + 1*256 = 1 + 4 + 128 + 256 = 389`

Hence the number in decimal is 389.

## Decimal to Other

Follow the same steps as described in [Decimal to Binary](conversion.md#Decimal%20to%20Binary), but divide the number by the base of the number system you want to convert to.

## Binary to Other
