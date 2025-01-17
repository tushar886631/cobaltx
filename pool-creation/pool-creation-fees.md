# Pool creation fees



{% tabs %}
{% tab title="CLMM pools" %}
There is no protocol fee for creating a CLMM pool. However, some Solana network and third-party fees apply:

&#x20;1\) Creation of a new Tick Array: 0.072 SOL

2\) Creation of a protocol position: 0.00245688 SOL

3\) Creation of an account to store personal position\*: 0.00284664 SOL

4\) Creation of the pool info 0.01163712 and vaults 0.00203928 SOL

5\) Creation and funding of the observation account: 0.03209256 SOL

6\) Creation of the NFT position (ATA)\*: 0.00203928 SOL

7\) Minting of the NFT and associated metadata: 0.00561672 SOL

8\) Metaplex protocol fee: 0.01 SOL. This amount may vary please refer to [Metaplex documentation](https://docs.metaplex.com/resources/protocol-fees).

9\) SOL network fee, and priority fee: <0,000007 SOL The average total is 0.1 SOL, this amount may however vary depending on the number of tick arrays initiated by the initial LP range.
{% endtab %}
{% endtabs %}

Note that it is impossible to close a pool once created. None of the fees mentioned above are refundable, except for those marked with \*.
