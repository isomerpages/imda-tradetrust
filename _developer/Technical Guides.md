---
title: Technical Guides
permalink: /developers/technical-guides/
variant: tiptap
description: ""
---
<p>Our response to some commonly encountered errors:</p>
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