---
layout:
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Position creation cost (CLMM)

There is no protocol fee for creating a CLMM pool position. However, some Solana network and third-party fees apply:

1\) Creation of a protocol position: 0.00245688 SOL

2\) Creation of an account to store personal position\*: 0.00284664 SOL

3\) NTF mint and (ATA)\*: 0.00277008 + 0.00207408 = 0.00484416 SOL

4\) SOL network fee, and priority fee: <0.000007 SOL The average net cost after closing the position is 0.00245688 SOL

Optional: when providing on a range including non-initiated ticks, a bitmap extension cost can occur. 5) Creation of a new Tick Array: 0.072 SOL - wide ranges can require multiple tick arrays None of the network fees mentioned above are refundable, except for those marked with \*.
