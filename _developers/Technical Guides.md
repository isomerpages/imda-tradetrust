---
title: Technical Guides
permalink: /developers/technical-guides/
variant: tiptap
description: ""
---
<p>Access step-by-step guide, additional tools and gallery of TradeTrust-issued
sample documents in <a href="https://docs.tradetrust.io/" rel="noopener noreferrer nofollow" target="_blank">TradeTrust technical guides.</a>
</p>
<h3><strong>Recommended guides :</strong></h3>
<table style="minWidth: 50px">
<colgroup>
<col>
<col>
</colgroup>
<tbody>
<tr>
<td rowspan="1" colspan="1">
<p></p>
</td>
<th rowspan="1" colspan="1">
<p></p>
</th>
</tr>
<tr>
<td rowspan="1" colspan="1">
<p>Documentation and guide for implementation</p>
</td>
<td rowspan="1" colspan="1">
<p><a href="https://docs.tradetrust.io/docs/getting-started" rel="noopener noreferrer nofollow" target="_blank"><sup>https://docs.tradetrust.io/docs/getting-started</sup></a>
</p>
</td>
</tr>
<tr>
<td rowspan="1" colspan="1">
<p>Transfer of holdership / ownership</p>
</td>
<td rowspan="1" colspan="1">
<p><a href="https://docs.tradetrust.io/docs/topics/introduction/transferable-records/title-transfer" rel="noopener noreferrer nofollow" target="_blank"><sup>https://docs.tradetrust.io/docs/topics/introduction/transferable-records/title-transfer</sup></a>
</p>
</td>
</tr>
<tr>
<td rowspan="1" colspan="1">
<p>Will be important to first understand Transferable Records</p>
</td>
<td rowspan="1" colspan="1">
<p><a href="https://docs.tradetrust.io/docs/tutorial/transferable-records/overview" rel="noopener noreferrer nofollow" target="_blank"><sup>https://docs.tradetrust.io/docs/tutorial/transferable-records/overview</sup></a>
</p>
</td>
</tr>
<tr>
<td rowspan="1" colspan="1">
<p>Address book management is an additional tool to help make sense of the
wallet addresses you might have from your partners</p>
</td>
<td rowspan="1" colspan="1">
<p><a href="https://docs.tradetrust.io/docs/reference/tradetrust-website/address-resolver/#address-book-local" rel="noopener noreferrer nofollow" target="_blank"><sup>https://docs.tradetrust.io/docs/reference/tradetrust-website/address-resolver/#address-book-local</sup></a>
</p>
</td>
</tr>
<tr>
<td rowspan="1" colspan="1">
<p>Get open-source code, including our reference implementation for the understanding
of framework's implementation</p>
</td>
<td rowspan="1" colspan="1">
<p><a href="https://github.com/tradetrust" rel="noopener noreferrer nofollow" target="_blank"><sup>https://github.com/tradetrust</sup></a>
</p>
</td>
</tr>
<tr>
<td rowspan="1" colspan="1">
<p>TradeTrust Open-source licensing terms</p>
</td>
<td rowspan="1" colspan="1">
<p><a href="https://github.com/TradeTrust/tradetrust-website" rel="noopener noreferrer nofollow" target="_blank"><sup>https://github.com/TradeTrust/tradetrust-website</sup></a>
<br><sup>click on Apache-2.0 license</sup>
</p>
<p></p>
<p></p>
</td>
</tr>
</tbody>
</table>
<p></p>
<p></p>
<h3><strong>Using TradeTrust with non-Ethereum blockchain</strong></h3>
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
<summary>The role of <a href="http://TradeTrust.io" rel="noopener noreferrer nofollow" target="_blank">TradeTrust.io</a> website</summary>
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
</div>
<p></p>
<p></p>
<p><a href="mailto:tradetrust@imda.gov.sg" rel="noopener noreferrer nofollow" target="_blank">Contact us for assistance!</a>
</p>
<p></p>
<p></p>
<p></p>