---
title: Common FAQs
permalink: /common-faqs/
variant: tiptap
description: Common FAQs for TradeTrust
third_nav_title: Product FAQ
---
<p></p>
<p>Why is the temporary domain created using TradeTrust Command Line Interface
not working?</p>
<p></p>
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