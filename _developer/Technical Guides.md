---
title: Technical Guides
permalink: /developer/technical-guides/
variant: tiptap
description: Access step-by-step guides, additional tools and gallery of
  TradeTrust-enabled sample documents in TradeTrust technical guides.
image: /images/TradeTrust logos/TT_LOGO_vertical.png
---
<p>Access step-by-step guides, additional tools and gallery of TradeTrust-enabled
sample documents in&nbsp;<a href="https://docs.tradetrust.io/" rel="noopener noreferrer nofollow" target="_blank">TradeTrust technical guides.</a>
</p>
<h4>Some recommended guides :</h4>
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
<td rowspan="1" colspan="1">
<p></p>
</td>
</tr>
<tr>
<td rowspan="1" colspan="1">
<p>Documentation and implementation</p>
</td>
<td rowspan="1" colspan="1">
<p><a href="https://docs.tradetrust.io" rel="noopener noreferrer nofollow" target="_blank">https://docs.tradetrust.io</a>
</p>
</td>
</tr>
<tr>
<td rowspan="1" colspan="1">
<p>Overview of Transferable Records</p>
</td>
<td rowspan="1" colspan="1">
<p><a rel="noopener noreferrer nofollow" target="_blank">https://docs.tradetrust.io/docs/tutorial/transferable-records/overview</a>
</p>
</td>
</tr>
<tr>
<td rowspan="1" colspan="1">
<p>Transfer of holdership / ownership</p>
</td>
<td rowspan="1" colspan="1">
<p><a rel="noopener noreferrer nofollow" target="_blank">https://docs.tradetrust.io/docs/topics/introduction/transferable-records/title-transfer</a>
</p>
</td>
</tr>
<tr>
<td rowspan="1" colspan="1">
<p>Address book management - an additional tool to manage the wallet addresses
of your partners</p>
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
<p><a rel="noopener noreferrer nofollow" target="_blank">https://docs.tradetrust.io/docs/reference/tradetrust-website/address-resolver/#address-book-local</a>
</p>
</td>
</tr>
<tr>
<td rowspan="1" colspan="1">
<p>Recommendations for wallet management</p>
</td>
<td rowspan="1" colspan="1">
<p>TradeTrust does not have any preferred wallet management. You may refer
to some solutions available in the market:</p>
<p><a href="https://docs.tradetrust.io/docs/topics/advanced/wallet-management/" rel="noopener noreferrer nofollow" target="_blank"><u>https://docs.tradetrust.io/docs/topics/advanced/wallet-management/</u></a>
</p>
</td>
</tr>
<tr>
<td rowspan="1" colspan="1">
<p>Storing of private keys and auto issue documents</p>
</td>
<td rowspan="1" colspan="1">
<p><a href="https://docs.tradetrust.io/docs/topics/advanced/aws-kms/overview" rel="noopener noreferrer nofollow" target="_blank">https://docs.tradetrust.io/docs/topics/advanced/aws-kms/overview</a>
</p>
</td>
</tr>
<tr>
<td rowspan="1" colspan="1">
<p>Get open-source code, including reference implementation to understand
the framework's implementation</p>
</td>
<td rowspan="1" colspan="1">
<p><a rel="noopener noreferrer nofollow" target="_blank">https://github.com/tradetrust</a>
</p>
</td>
</tr>
<tr>
<td rowspan="1" colspan="1">
<p>TradeTrust Open-source licensing terms</p>
</td>
<td rowspan="1" colspan="1">
<p><a href="https://github.com/TradeTrust/tradetrust-website?tab=Apache-2.0-1-ov-file#readme" rel="noopener noreferrer nofollow" target="_blank">Apache-2.0 license</a>
</p>
</td>
</tr>
<tr>
<td rowspan="1" colspan="1">
<p></p>
</td>
<td rowspan="1" colspan="1">
<p></p>
</td>
</tr>
</tbody>
</table>
<p></p>
<h4>Responses to some commonly encountered errors:</h4>
<div data-type="detailGroup" class="isomer-accordion isomer-accordion-white">
<details class="isomer-details">
<summary>Why is the temporary domain created using TradeTrust Command Line Interface
not working?</summary>
<div data-type="detailsContent" class="isomer-details-content">
<p>The temporary domain is only valid for 24 hours.</p>
</div>
</details>
<details class="isomer-details">
<summary>What should I do when I encounter an error while verifying a document?
And what does each error mean?</summary>
<div data-type="detailsContent" class="isomer-details-content">
<p>There are mainly three types of errors that can occur when verifying a
document:</p>
<ol data-tight="true" class="tight">
<li>
<p><u>Document not issued:</u> TradeTrust checks that the document has been
issued and that its issuance status is in good standing. This error occurs
if the issuer revokes the document or if it has not been issued.</p>
</li>
<li>
<p><u>Document issuer's identity is invalid</u>: TradeTrust validates the
the issuer's idenity. This error occurs if the document was issued by someone
whose identity could not be verified.</p>
</li>
<li>
<p><u>Document has been tampered with</u>: TradeTrust ensures that the document's
contents remain unchanged since its creation, except for data removed using
the built-in obfuscation mechanism. This error occurs if the document's
content has been modified.</p>
</li>
</ol>
<p>If you encounter any of these errors, please contact the <strong>document issuer</strong> for
assistance.</p>
<p></p>
</div>
</details>
</div>
<p></p>
<blockquote>
<p>To reach our tech support, <a href="https://github.com/TradeTrust/tradetrust-core/issues" rel="noopener noreferrer nofollow" target="_blank">create an issue</a> or
<a href="https://form.gov.sg/635f32c5001b2d0011fff09b" rel="noopener noreferrer nofollow" target="_blank">contact us</a>.</p>
</blockquote>
<p></p>
<p></p>
<p></p>