---
description: How to give the power to the chosen few?
---

# From POS to POA

PWr coin's goal is to allow students within an university to exchange currecny under supervision of university's authorities. We decided, that there should be special nodes, that will authoritize transactions, that will be trusted by all participants - this means at least one authority node within a univeristy. Only one model of blockchain proof meets this demand - proof of authority.

Since we based our coin on NXT - an open source cryptocurrency written in Java and working under proof of stake’s model – we had to change it’s source code to fit our requirements. It turned out, however, to be a tough nut to crack.

For blockchain, given proof is one of the most essential features of whole system. Hence it wasn’t a surprise, that under NXT’s hood there was plenty of references to it’s proof od stake’s model. We tried to locate them and modify.

First of all, we added IP address of example authority node for our network in configuration file for the project. This might work well as long as the IP addresses are not changed. Every user in the network would have access to them. 

![](../.gitbook/assets/obraz%20%282%29.png)

Next we had to find where is the code responsible for validating transactions and modify it to assure that all transactions are being validated only by authority nodes. Where could it be…?

Well, that seemed to be close… 

![](../.gitbook/assets/obraz.png)

  
Then we implemented an instance that will direct all validations into our authority node. 

![](../.gitbook/assets/obraz%20%283%29.png)

Having this, all we had to do was to call this method in the right place: 

![](../.gitbook/assets/obraz%20%281%29.png)

  
And implement the actual working transaction interceptor: 

![](../.gitbook/assets/obraz%20%284%29.png)

	

This was all not without a problems. IP in local network is changing frequently, and hardcode’ing it was a poor idea. Not to mention problems with retrieving own local ip addresses from given network.

Above all, there was problems with NXT itself. Implementing proof of authority on top of proof of stake was difficult due the scattered all over the source code logic directly designed to work under proof of stake. Multiple classes having hundreds of lines of code were written only in purpose of serving proof of stake logic. What we’ve done here was only an interim solution that would not work under highly exploited network where efficiency and reliability requirements would be much higher. Eventually we’ve claimed that implementing PoA at top of NXT is uneconomic due the necessity of turning coin’s architecture upside down. 

