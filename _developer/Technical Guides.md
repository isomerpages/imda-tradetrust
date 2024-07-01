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
<p>TradeTrust leverages on different types of identifier resolvers:</p>
<ol data-tight="true" class="tight">
<li>
<p>Local Address Book (flat file to map one identifer to another)</p>
</li>
<li>
<p>Third Party REST APIS (conforming to TT specs)</p>
</li>
</ol>
<p></p>
<p><a href="https://docs.tradetrust.io/docs/reference/tradetrust-website/address-resolver/#address-book-local" rel="noopener noreferrer nofollow" target="_blank"><sup>https://docs.tradetrust.io/docs/reference/tradetrust-website/address-resolver/#address-book-local</sup></a>
</p>
</td>
</tr>
<tr>
<td rowspan="1" colspan="1">
<p>TradeTrust does not have any preferred wallet management. You may refer
to some solutions available in the market</p>
</td>
<td rowspan="1" colspan="1">
<p><a href="https://docs.tradetrust.io/docs/topics/advanced/wallet-management/" rel="noopener noreferrer nofollow" target="_blank"><u>https://docs.tradetrust.io/docs/topics/advanced/wallet-management/</u></a>
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
<p>Some commonly encountered errors:</p>
<div data-type="detailGroup" class="isomer-accordion isomer-accordion-white">
<details class="isomer-details">
<summary>Why is the temporary domain created using TradeTrust CLI not working?</summary>
<div data-type="detailsContent" class="isomer-details-content">
<p>The temporary domain is only valid for 24 hours.</p>
</div>
</details>
<details class="isomer-details">
<summary><strong>While verifying a document, what should I do when I encounter an error, and what does each error mean?</strong>
</summary>
<div data-type="detailsContent" class="isomer-details-content">
<p>There are mainly three types of errors that can occur when verifying a
document:</p>
<ol data-tight="true" class="tight">
<li>
<p>Document not issued: TradeTrust checks that the document has been issued
and that its issuance status is in good standing. This error occurs if
the issuer revokes the document or if the document has not been issued.</p>
</li>
<li>
<p>Document issuer identity is invalid: TradeTrust validates and returns
the identity of the issuer. This error occurs if the document was issued
by an invalid user.</p>
</li>
<li>
<p>Document has been tampered with: TradeTrust ensures that the content of
the document remains unchanged since its creation, except for data removed
using the built-in obfuscation mechanism. This error occurs if the document's
content has been modified.</p>
</li>
</ol>
<p>If you encounter any of these errors, please contact the document issuer
for assistance.</p>
<p></p>
</div>
</details>
</div>
<p></p>
<blockquote>
<p>To reach our tech support, <a href="https://github.com/TradeTrust/tradetrust-core/issues" rel="noopener noreferrer nofollow" target="_blank">create an issue</a> or
&lt;contact us&gt;!</p>
</blockquote>
<p></p>
<p></p>
<p></p>