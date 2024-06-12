---
title: Blockchain Guideline
permalink: /blockchain-guideline/
variant: tiptap
description: ""
---
<p></p>
<div data-type="detailGroup" class="isomer-accordion isomer-accordion-white">
<details class="isomer-details">
<summary>The role of blockchain and Ethereum in TradeTrust</summary>
<div data-type="detailsContent" class="isomer-details-content">
<p>The reason that a blockchain is used in TradeTrust is to eliminate the
problem of "whose database should we use", especially in situations of
multipartite sovereign nation involvement or even competitive industry
giants. The responsibilities behind the operation and custody of this database
includes maintaining ownership records of title document and ensuring the
correctness of ownership transitions, providing the necessary infrastructure
that all parties can access, and so on. One of the key design principles
of TradeTrust is that no central authority should be managing these transaction
records. Instead of solving the no-win scenario of agreeing on the party
who should be entrusted with these responsibilities, we have shifted this
responsibility to the neutral and impartial consensus mechanism that is
innate to blockchains.</p>
<p>Since blockchains are capable of providing immutable records of transactions
and the current state, they can be used to provide a rail for keeping records
for Electronic Transferable Records (ETRs).</p>
<p>TradeTrust requires the underlying technology to support the 2 categories
of trade documents:</p>
<ol data-tight="true" class="tight">
<li>
<p><strong>Transferable documents:</strong> Trade documents that entitle the
holder to claim the performance of an obligation or ownership (e.g. bills
of lading, bills of exchange, etc.) and the selected blockchain needs to
be able to track and transfer ownership of the trade document.</p>
</li>
<li>
<p><strong>Normal documents/Verifiable documents:</strong> Other non-transferable
trade documents that do not confer ownership&nbsp;(e.g. invoices, packing
list, certificate of origin, etc.). These trade documents can be verified
for its authenticity, integrity and provenance.</p>
</li>
</ol>
<p>The current implementation of TradeTrust is using the Ethereum blockchain
whereby the ERC-721 provides a widely-used smart contract API used on non-fungible
tokens to allow transfer of ownership whilst providing assurance of integrity,
singularity and control.</p>
</div>
</details>
<details class="isomer-details">
<summary>The role of TradeTrust website</summary>
<div data-type="detailsContent" class="isomer-details-content">
<p>The website at <a href="https://www.tradetrust.io/" rel="noopener noreferrer nofollow" target="_blank">https://www.tradetrust.io</a> serves
as:</p>
<ol data-tight="true" class="tight">
<li>
<p>reference implementation on the TradeTrust framework with an intuitive
user interface to demonstrate the core capabilities; and</p>
</li>
<li>
<p>a neutral mechanism to self-check for interoperability.</p>
</li>
</ol>
<p>The TradeTrust reference implementation offers the available functions
of the TradeTrust framework. It lets users try out how digital trade documents
are issued using TradeTrust and how transferable records such as the electronic
Bill of Lading (eBL) can be created. This free and neutral interface can
also be used to quickly verify the authenticity and provenance of a document
issued in such a manner.</p>
<p>For instance, if a user drops a TradeTrust-created eBL onto the website
and sees that it has been issued by <a href="https://www.tradetrust.io/" rel="noopener noreferrer nofollow" target="_blank">www.pilship.com</a>, he can be assured
that it is a legitimate eBL from Pacific International Lines (on the assumption
that the entity owns the said domain). In this approach, the user can simplify
the trust model to "if issuer domain is an entity I know and trust, I can
then be assured that the contents of the document is authentic and legitimate
".</p>
</div>
</details>
<details class="isomer-details">
<summary>Mandatory properties of a blockchain</summary>
<div data-type="detailsContent" class="isomer-details-content">
<p>One of the most frequently asked questions posted to the team is whether
TradeTrust is able to use alternative blockchains in addition to the Ethereum
blockchain. This article seeks to provide a set of guidelines on the properties
and features that an alternative blockchain must have in order to align
to the TradeTrust framework.</p>
<p><strong>Here is a list of mandatory properties:</strong>
</p>
<p><strong>1. Public</strong>
</p>
<p>The blockchain shall be safe, accessible, and auditable for all participants.
Selecting a public blockchain prevents fragmentation of the network by
discouraging solution providers to use a private network which locks their
end user into a small ecosystem and encourages interoperability of software
from different solution providers to agree on document schema, valid state
transition actions and best practices.</p>
<p><strong>2. Supports NFTs/Smart Contracts</strong>
</p>
<p>The selected blockchain shall minimally support arbitrary digital asset
ownership structures, and ideally be support <strong>Turing Complete Smart Contracts.</strong> In
order to fulfil the requirement of asset ownership capability, it must
be able to:</p>
<ol data-tight="true" class="tight">
<li>
<p>Define a unique digital asset</p>
</li>
<li>
<p>Singularly keep ownership records of instances of digital assets</p>
</li>
<li>
<p>Allow an owner to prove control over the digital asset</p>
</li>
</ol>
<p>For additional flexibility, it would be ideal for the blockchain to support
smart contracts that allow actors to define a valid set of state transitioning
transactions, their preconditions and post-conditions. This is needed for
programs like the DocumentStore, TokenRegistry or TitleEscrow to store
information about the states of documents and ownership structure. An example
of how smart contracts are used: In the case of ETR issuers such as shipping
lines, they should be able to deploy smart contracts to maintain a single
global record for the following purposes:</p>
<ul data-tight="true" class="tight">
<li>
<p>Keeping records of the statuses of ETRs issued by the issuer</p>
</li>
<li>
<p>Keeping records of the current owners of the different ETR</p>
</li>
<li>
<p>Defining the function and preconditions for issuing a new ETR</p>
</li>
<li>
<p>Defining the function and preconditions for transferring an ETR</p>
</li>
<li>
<p>Other functions required by the users or the issuer of the ETR</p>
</li>
</ul>
<p>Example of how preconditions are set for a transfer action: An entity
may only transfer its ownership of an ETR from itself to another entity&nbsp;only
if the following pre-conditions are met:</p>
<ul data-tight="true" class="tight">
<li>
<p>The ETR has been issued by the ETR issuer</p>
</li>
<li>
<p>The Entity is currently in control</p>
</li>
<li>
<p>The transaction has been signed by the entity proposing the transactions</p>
</li>
</ul>
<p><strong>3. Accessibility of blockchain state</strong>
</p>
<p>TradeTrust requires the blockchain to satisfy the accessibility criteria
below:</p>
<ol data-tight="true" class="tight">
<li>
<p><strong>availability:</strong> any party can download and verify the current
head state meaning it is censorship-resistant</p>
</li>
<li>
<p><strong>safety/validity:</strong> must not have invalid state transition</p>
</li>
<li>
<p><strong>liveness:</strong> any party can submit transactions to advance
the head state</p>
</li>
</ol>
<p><strong>4. Impartial Security Model</strong>
</p>
<p>The set of entities that are allowed to append blocks to the blockchain
should be <strong>large enough</strong> such that the <strong>possibility of bribery</strong> or <strong>colluding</strong> among
critical node operators is nearly impossible. If collusion occurs, it shall
be detectable by any participants in the system. The membership criteria
for this set of entities must not exclude actors based on subjective factors
(e.g political, geographic, social). This allows the security of the network
to be objectively measured in terms of crypto-economics – i.e the cost
of a successful attack on the network should be definitive. It also ensures
that any interested actor should be able to join the validator set, such
that no party should be able to veto or deny service to any other. For
private blockchains, the possibility of collusion or a buy-out scenario
among the node players are higher due to the smaller number of players.</p>
<p><strong>5. Economically Secured</strong>
</p>
<p>The blockchain needs to <strong>continue to operate</strong> even if some
nodes fail or act maliciously. That is, the cost of an attack should far
outweigh any possible gains from a successful attack. The cost of an attack
on the blockchain could be used as a proxy to evaluate if such an economic
opportunity could be present. One plausible attack scenario is the rent-to-pwn
scenario, where smaller public, permissionless proof-of-work blockchains
are attacked simply by mercenary actors that put up their computational
power for sale. This eliminates the security of many ledgers that are secure
in theory if they have the majority of all proof-of-work that exists in
the universe, but falls apart if they are not.</p>
<p><strong>6. Open-sourced</strong>
</p>
<p>The blockchain shall be an <strong>open-source software</strong> (OSS) that
is open for public review. This is important to ensure that participants
have the chance to review the underlying code prior to partaking in any
activities on the blockchain in the spirit of "Don't Trust, Verify". Necessarily,
this implies that the protocol and consensus mechanisms are all public
and easily verifiable as well.</p>
<p>The guidelines offer insights into what the TradeTrust framework and reference
implementation look for in terms of its choice of blockchains. The properties
of a blockchain must satisfy the requirements stipulated in the MLETR:</p>
<ol data-tight="true" class="tight">
<li>
<p><strong>Singularity:</strong> The ETR document can be represented by an
unique Document ID which cannot collide with another document and the association
of the ID to a single <code>owner</code> property in a smart contract ensures
that there is only one owner of the ETR at any point in time.</p>
</li>
<li>
<p><strong>Exclusive Control:</strong> The implementation of the ETR smart
contract can be implemented such that the listed owner of the ETR will
have exclusive control over the ETR. This means that only the owner of
the ETR can invoke the transfer function of the ETR and the signature of
the transfer transaction is being checked to assert the constraints.</p>
</li>
<li>
<p><strong>Integrity:</strong> Integrity of an ETR can be verified through
an unique Document ID that is the hash of the content of the document.
Any attempt to modify the contents of the document will result in the document
hash to change thus giving recipients of the ETR, assurance as to the integrity
of the document.</p>
</li>
</ol>
</div>
</details>
<details class="isomer-details">
<summary>Other preferred properties of a blockchain</summary>
<div data-type="detailsContent" class="isomer-details-content">
<p>In addition, here are properties that are preferred and recommended for
easier alignment and integration to the TradeTrust framework.</p>
<p><strong>1. Actively maintained with a large development community</strong>
</p>
<p>In order for key vulnerabilities to be fixed, the blockchain needs to
be <strong>actively maintained</strong> by a distributed set of engineers.
In addition, formal guidelines for contributions and code review process
should be present to protect against malicious code contributions.</p>
<p><strong>2. Have withstood the test of time</strong>
</p>
<p>The blockchain should ideally also be running on a network which has <strong>withstood against the test of time</strong> where
other transactions involving large values are being processed and have
shown resilience against malicious actors. As the foundation of the application
stack as a global state provider, a failure at this layer would be catastrophic.</p>
<p><strong>3. Ethereum Virtual Machine (EVM) Compatible</strong>
</p>
<p>The blockchain should preferably be EVM compatible to allow the users
to leverage TradeTrust’s existing smart contract codebase without having
to make drastic re-implementations.</p>
</div>
</details>
<details class="isomer-details">
<summary></summary>
<div data-type="detailsContent" class="isomer-details-content">
<p></p>
</div>
</details>
</div>
<h4>An open invitation to developers</h4>
<p>The Ethereum main network is currently the canonical blockchain for our
reference implementation at our website - <a href="https://tradetrust.io/" rel="noopener noreferrer nofollow" target="_blank">tradetrust.io</a> . Ethereum remains our choice
of a data backend as it allows for permissionless onboarding, and minimises
any quarrels over ownership of the infrastructure. Ethereum 2.0 offers
a promising solution that is scalable and addresses some environmental
concerns, but it is currently not yet ready.</p>
<p>Moving forward, other suitable blockchains that have the mandatory properties
and features may be considered to be offered as alternative options for
the TradeTrust framework. The conditions will serve as a guideline to identify
suitable candidates for consideration. We’d like to invite you to work
with us to expand the list of blockchain options for TradeTrust. Feel free
to <a href="https://www.form.gov.sg/635f32c5001b2d0011fff09b" rel="noopener noreferrer nofollow" target="_blank">contact us</a> to
discuss further.</p>