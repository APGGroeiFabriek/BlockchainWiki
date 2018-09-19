# Blockchain – Legal context

_Edited by André Zandee_
_Created 7 Sept 2018_

Any disruptive new technology encounters issues with the legal context matching the existing situation. This is not different for Blockchain.

On the other hand, Blockchain could also create new possibilities in the field of Legal context, in the sense of new ways of sharing information.

This wiki is not intended to provide you with a complete listing of legal challenges, nor to give you legal advice or any other angle which could lead to claims. We want to provide you some insights on topics which are known at the moment of writing this are precarious when defining new Blockchain-solutions and thus require further, professional, legal advice.

## Challenges: Technical Setup

The technical setup of Blockchain creates friction with the recently activated GDPR-laws. The main issues here are:


<table>
  <tr>
   <td><strong>Technical setup</strong>
   </td>
   <td><strong>GDPR conflicts</strong>
   </td>
  </tr>
  <tr>
   <td>BC stores all transactions ever registers
   </td>
   <td rowspan="2" >Conflicts with Art. 17 GDPR Right to erasure ('right to be forgotten').
<p>
No good solution has been found, but directions for this could be:<ul>

<li>Make link between entity-record unfindable (Throw away the key)
<li>Make data unreadable (replace data with hash)</li></ul>

   </td>
  </tr>
  <tr>
   <td>Immutability of records
   </td>
  </tr>
  <tr>
   <td>Peer-to-peer technology requires every node to contain a partial or complete data-set
   </td>
   <td rowspan="2" >GDPR defines any party handling or storing data as a data-processor
<p>
GDPR requires of a data-processor of Personal Data (GDPR art 32):<ul>

<li>A direct (business)necessity  to handle or store this data in the form of an explicit Agreement / Instruction from the Data-Controller
<li>Sufficient organizational/operational security-measures to protect this data
<li>Notification of any data-leaks as soon as they occur

<p>
This is not possible in a peer-to-peer platform, especially when it's a public/permissionless network (anyone can join without KYC on nodes).
<p>
Solutions:<ul>

<li>JP Morgan's Qorum provides a possibility to define whether a node receives the full data or only the hash.
<li>Furthermore there's a number of solutions in the making to store data in IPFS-like depositories, but this is no solution for the data-processing issue….</li></ul>
</li></ul>

   </td>
  </tr>
  <tr>
   <td>Public Blockchain: Trustless & Anonymous parties
   </td>
  </tr>
  <tr>
   <td>At this moment limited interchain-connections
   </td>
   <td>GDPR states that the data subject (person who's personal data is stored) has the right to demand all of his/her data is transported to another platform  (art 20: Right to data portability). 
<p>
At this moment Blockchains are not interlinked (yet). GDPR does not exactly stipulate to what respect a data subject can determine platform, data format, etc, etc.
   </td>
  </tr>
</table>


## Challenges: Business Model**

There are also some functional characteristics of Blockchain-implementations which conflict with current day law as well.


<table>
  <tr>
   <td><strong>Business Model feature</strong>
   </td>
   <td><strong>GDPR conflicts</strong>
   </td>
  </tr>
  <tr>
   <td>Geographical scope roll-out
   </td>
   <td rowspan="2" >Blockchain, like any other internet-based technology, has at the basis a global reach.
<p>
When implemented and available for customers worldwide, the Blockchain-implementing company needs to keep in mind that he/she needs to comply to any of the legal requirements of the geographical jurisdictions in which potential customers reside.
   </td>
  </tr>
  <tr>
   <td>
   </td>
  </tr>
  <tr>
   <td>Crypto currency
   </td>
   <td rowspan="2" >National governments want to keep control over the monetary system within their territory; in fact anything representing financial products is usually controlled.
<p>
Blockchain tokens can be used for either functionalities in the direction of a crypto-currency, tokenized assets or to collect money for an ICO.
<p>
For a lot of countries this means that the bank, securities, securities trading, and/or anti-money-laundering-laws be applicable.
<p>
Some examples are: Switzerland/<a href="https://www.finma.ch/en/documentation/finma-guidance/">FINMA</a>, Germany/<a href="https://www.bafin.de/EN/Aufsicht/FinTech/Blockchain/blockchain_node_en.html">BaFin</a>, Netherlands/<a href="https://www.afm.nl/en/professionals/onderwerpen/ico">AFM</a>
   </td>
  </tr>
  <tr>
   <td>ICO
   </td>
  </tr>
  <tr>
   <td>Realizing Blockchain's business value
   </td>
   <td>Blockchain can bring a platform to redefine business processes. Legislation defines boundaries of norms and values, right and wrong, roles and responsibilities to keep checks and balances, around historical and hopefully current operational state of affairs. 
<p>
When a disruptive new technology is being introduced, the possibilities usually start shifting, and so do the roles and responsibilities.
<p>
Current legislation usually is too restrictive and poses a blockages around this redefinition of tasks and roles.
<p>
An example:
<p>
Blockchain brings transparency. Within legislation a lot of legal text is around processes currently required to bring and secure this transparency.
   </td>
  </tr>
</table>


## Opportunities

Blockchain can be seen as a peer-to-peer data sharing platform, whereby transparency and privacy are programmable.

At this moment there's a lot of Chinese walls being defined to rigidly protect  the personal privacy.

An example: The use of medical data. When the police need to act towards a specific individual, this medical data could be of vital importance in their approach. The police, not being a medical organization,  is legally forbidden to process this (GDPR art 9). The only reason they are allowed to do so, is when this could prevent a life-threatening situation. Unfortunately this is not always known upfront….

What could be a blockchain-solution, is to have a blockchain, nodes both at the side of the police and medical institutions, where the police could request information to [an oracle](https://blockchainhub.net/blockchain-oracles/) within premises of the medical organization. The oracle validates the question, the medical situation and when of vital importance, converts the medical information into a police-usable information-set and communicates back.

As mentioned before, still some legal hurdles need to be tackled within this field to realize these type of bringing together worlds through blockchain.