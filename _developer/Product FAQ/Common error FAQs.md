---
title: Common error FAQs
permalink: /common-error-faqs/
variant: tiptap
description: FAQs for common errors encountered during implementation of TradeTrust
third_nav_title: Product FAQ
---
<p></p>
<table style="minWidth: 25px">
<colgroup>
<col>
</colgroup>
<tbody>
<tr>
<th rowspan="1" colspan="1">
<p></p>
</th>
</tr>
<tr>
<td rowspan="1" colspan="1">
<ol data-tight="true" class="tight">
<li>
<p>Why is the temporary domain created using TradeTrust Command Line Interface
not working?</p>
<p>The temporary domain is only valid for 24 hours.</p>
</li>
</ol>
</td>
</tr>
<tr>
<td rowspan="1" colspan="1">
<ol start="2" data-tight="true" class="tight">
<li>
<p>There are mainly three types of errors that can occur when verifying a
document:</p>
</li>
</ol>
<ul data-tight="true" class="tight">
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
</ul>
<p></p>
<p>If you encounter any of these errors, please contact the <strong>document issuer</strong> for
assistance.</p>
</td>
</tr>
<tr>
<td rowspan="1" colspan="1">
<p></p>
</td>
</tr>
</tbody>
</table>
<p></p>