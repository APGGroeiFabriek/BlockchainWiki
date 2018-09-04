# Consensus

by: Dean Masley | September 4, 2018

![](https://cdn-images-1.medium.com/max/1600/1*9Uhf9Kp12ueoce1CQPd6bw.png)

## In a Nutshell

Traditionally, when you want to use an internet service, you connect to a server run by a company. This server maintains the databse of information that you can access by downloading the app. All decisions relating how to manipulate the database, such as adding records, editing information, or deleting content is made by the company running the server. It is their responsibility to ensure the server represents the genuine truth.

Let's take the example of paypal:
1.  You wish to send money to a friend using paypal
2.  You signup on paypal.com, which paypal will approve and add you to their servers.
3.  You deposit money to paypal's bank account, and then they will add a transaction on their database showing your new balance. This balance is simply credit that paypal owes you.
4.  You send money to your friend using paypal. Paypal makes a new record on their database which debits your balance and credits your friend's wallet.

Then the anonymous creator of Bitcoin, Satoshi Nakamoto, came up with an astounding innovation: a ledger that doesn't require a central server or authority to maintain it.

While a rudimentary example: the bitcoin blockchain is equivalent to multiple computers running the same excel file at the same time. Thus, you need rules to decide how new records (such as deposits, transfers, withdraws) would be handled, ensuring against malicious edits. Afterall, the ledger only has integrity and use if people trust it to be valid. The important decisions about how to manipulate the database is now done as a group instead of trusting someone else to do it for us. 

## Mining

You may have heard of the term "mining". A miner is the actor who validates and adds transactions to the ledger within a *Proof of Work* (PoW) coin, such as Bitcoin. There's several actors involved within a PoW regime, with a seperation of powers in play for each group to check the power of another.

* Miners maintain the physical equipment, nodes, and computers that provide the computational effort to process transactions and secure the ledger. They spend money on the equipment itself and the large energy bills created while running these machines. As a reward, they compete for the block reward every 10 minutes. The block reward is currently 12.5 Bitcoin.
* Developers create and improve the code that's being run on all the miners and user's machines. They don't have any higher access to the ledger than the user. Miners and users check their power by deciding if they run their software or not.
* Users cause the bulk of transactions. These are the enthusiasts using the software in the real world, deploying it to solve problems (often their own). Without users, there would be no audience for the miners or developers to create for. Users hold power of deciding which solutions are relevant. 

Each group within the PoW system provides services to the other, and has leverage to check any one group trying to abuse their position. These natural rewards and punishments, game theory, stablize the decentralized group of people using, developing, and running the coin.

## Types of Consensus

Proof of Work is not the only way to organize a group of people to run a distributed system. Think of these consensus mechanisms as simply the rules how the group decides on the next series of transactions, and how to ensure they aren't malicious. While PoW is considered the most secure and battletested, it has a few draw backs:

**Proof of Work**
* Requires physical computers to run resource intensive processes in order to “vote” on the next block of transactions to be added to chain.
* This requirement of physical machines that consume a lot of energy is to make attacking the system costly. Thus even bad actors have an economic incentive to follow the rules because once they do, they will start earning money instead of gaining nothing by hacking it.
* Drawback: This consumes a lot of energy. While a plurality of miners use [renewable energy sources](https://cointelegraph.com/storage/uploads/view/63c09c4f88dee4a6153eb4020dd8360e.png), this isn't sustainable and we should find less resource intensive ways to secure our software from malicious actors.


<table>
  <tr>
   <td>Type
   </td>
   <td>Mechanism
   </td>
   <td>Drawbacks
   </td>
  </tr>
  <tr>
   <td>Proof of Work `PoW` <br><br>[🎥](https://youtu.be/9V1bipPkCTU)
   </td>
   <td>Requires physical computers to run resource intensive processes in order to process the next block of transactions to be added to chain. <br><br> This requirement of physical computers doing processes that require a lot of energy ensures against malicious actors spending real world money to purchase a large enough warehouse of computers to 
   </td>
   <td>This consumes a lot of energy. While a plurality of miners use [renewable energy sources](https://cointelegraph.com/storage/uploads/view/63c09c4f88dee4a6153eb4020dd8360e.png), this isn't sustainable and we should find less resource intensive ways to secure our software from malicious actors.
   </td>
  </tr>
  <tr>
   <td>Proof of Stake `PoS` <br><br> [🎥](https://youtu.be/M3EFi_POhps)
   </td>
   <td>Requires large holders of the coin to put them 'at stake' for the privilege of adding the next block of transactions. The network chooses at random, weighted by amount of coin held.<br><br>
   	This removes the physical component and instead uses an individual's investment in the ecosystem as the balance of power. Someone would be required to purchase a large percentage of total coins, with the self-defeating intent to make the coin worthless by maliciously attacking it.
   </td>
   <td>Assumes the holders of coin are driven by purely economic needs. A malicious actor with large sums of money could more easily gain influence.
   </td>
  </tr>
  <tr>
   <td>Delegated Proof of Stake `DPoS` <br><br> [🎥](https://youtu.be/ERVxhzaRbVY)
   </td>
   <td>Like a representative democracy, everyone votes on the validators of the newtork to represent their interests. Similar to proof of stake, except instead of anyone being able to stake, except only a selected group of validators are voted in to mint the next group of blocks.<br><br>Aims to reduce the ability for malicious actors to take control of the chain while maintaining fast speeds and not need miners.
   </td>
   <td>By reducing the group of validators to a trusted group, centralization concerns begin to creep in.
   </td>
  </tr>
  <tr>
   <td>Proof of Burn `PoB`
   </td>
   <td>Using an existing blockchain, users could send their coin to a wallet which is unlikely anyone has the key too. Thus, the coins sent to this wallet are essentially lost forever, or "burned". This allows the creation of a new asset that can only be created by destroying another coin (basically converting it). 
<p>
This creates the friction needed to prevent anyone from making a ton of coins, allowing natural economies to develop. 
   </td>
   <td>This process purposefully destroys coin that can never be used again. Additionally, while the process seems similar to an ICO, the funds converted aren't available to the developers. This prevents conflict of interest but also prevents developers from having cashflow to work on the project full time.
   </td>
  </tr>
  <tr>
   <td>Practical Byzantine Fault-Tolerant `PBFT`
   </td>
   <td>Useful for enterprise situations where you have a small group of participants that need to share a database. Doesn't require hashing or wasting energy to process a higher volume of transactions.
   </td>
   <td>Not a practical consensus mechanism for open and permissionless systems. 
   </td>
  </tr>
  <tr>
   <td>Proof of Identity `PoI`
   </td>
   <td>The purpose of consensus mechanisms is to give everyone the ability to vote on the next series of transactions. This problem is not an issue if every participant has a legitimate and vested identity. 
<p>
If everyone could vote on the next series of blocks, we wouldn't need as many other mechanisms to ensure trust amongst anonymous participants.
   </td>
   <td>There doesn't exist a universal identity system to pull this off in any sizeable scale.
   </td>
  </tr>
</table>

## More Links
* [🎥 How Bitcoin Works Under the Hood](https://youtu.be/Lx9zgZCMqXE)
* [📄 PoW vs PoS](https://hackernoon.com/consensus-mechanisms-explained-pow-vs-pos-89951c66ae10)
* [🎥 Life inside a chinese bitcoin mine](https://youtu.be/K8kua5B5K3I)
* [🎥 Andreas Antonopoulos: Rules without Rulers](https://youtu.be/2tqo7PX5Pyc)
* [📄 Alternative Consensus Algorithms](https://hackernoon.com/alternative-blockchain-consensus-mechanisms-40c1509af39e)
* [📄 Private vs Public Blockchains](https://blog.ethereum.org/2015/08/07/on-public-and-private-blockchains/)

*other consensus content coming soon*


