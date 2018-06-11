# Features

#### Privacy - who is allowed to participate in network?

Possible solutions- anyone can join network- potential participants need an invitation or permission \(for example every student with valid identity card is permitted to join the network\)- existing participants could decide future entrants- consortium could make the decisions- regulatory authority could issue licenses for participation.

{% hint style="info" %}
Project is dedicated to scientific institutions so transactions should be transparent for all network participants by definition.
{% endhint %}

## Hashing Algorithm

A hash function is a step-by-step mathematical procedure that converts data of any length into data of a fixed, short length. Hashing method is the main security of cryptocurrency, used for securing each and every block. Litecoin uses Scrypt, which is fast and specificaly designed for the coin, but it is not as well tested as other algorithms, so it may expose some dangers in the future. We decided to use SHA256-3. It is the newest version of Secure Hashing Algorithm released in 2015 and it provides security at the top level. Software implementation might be slower than some other solutions, but since our coin is developed for smaller community, the performance issues are not playing such an important role.

**Scrypt**

* Litecoin uses a simplified version of Scrypt
* Initially designed to make it costly to perform large-scale custom hardware attacks
* Less widely used and analyzed than the SHA2 hashing algorithm used in Bitcoin, so there is some concern about possible weaknesses in its cryptographic scheme being discovered in the future

**X11**

* Composite function of multiple hashing algorithms
* The algorithm uses eleven hashing functions from the Blake algorithm to the Keccak algorithm making it very secure
* Algorithm is not as long-term as some expect it to be. Some scientists give it a maximum of two years before this algorithm gets ASIC’d

**SHA3-256**

* Quantum-proof, should last billions of years,
* Used by POA network, other Proof Of Authority network- probably best choice right now.

{% hint style="info" %}
NXT uses SHA-256, so PWrCoin's hashing algorithm is SHA-256.
{% endhint %}

## Mining

Mining is using computing power to solve mathematical problem and produce a block. Mining is the basis for proof-of-work cryptocurrencies.

{% hint style="info" %}
Since chosen proof is Proof of Authority, there will be no mining in our coin. This will also provide good transaction time.
{% endhint %}

## Mining time

> _In private networks, a block time as low as three seconds works well._ ~ Building Blockchain Projects by Naryan Prusty

## Maximum supply

Maximal possible amount of coins existing on the market. 

{% hint style="info" %}
For PWr Coin we decided it to be 1 000 000.This is pretty, round number for calculating and statistics purposes.
{% endhint %}

## Block time

Block time is the length of time between the generation of each new block. 

{% hint style="info" %}
The average block time in NXT is ~1.5 minutes, in PWrCoin - it will be 1 minute.
{% endhint %}

##  Block size

Block size is the memory required to store a full block. In NXT, this is 32kB.  




