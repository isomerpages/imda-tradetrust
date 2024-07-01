---
title: What is the DID approach in TradeTrust?
permalink: /developers/product-faq/did-approach/
variant: tiptap
description: ""
third_nav_title: Product FAQ
---
<p>Decentralized identifiers (DIDs) enable businesses to establish trust
and verify the authenticity of digital identities without relying on a
central authority. This can be particularly useful for secure and efficient
interactions with customers, partners, and other entities, while giving
the business more control over its digital identity infrastructure.</p>
<p>The DID approach in TradeTrust makes use of DIDs to allow our document
issuance flow to not rely on the need to write on blockchain thus eliminating
the need for gas fees. For more information:</p>
<p><a href="https://docs.tradetrust.io/docs/topics/introduction/issuer-method-dns-did" rel="noopener noreferrer nofollow" target="_blank">https://docs.tradetrust.io/docs/topics/introduction/issuer-method-dns-did</a>
</p>
<p>By design, DID approach is only applicable for verifiable documents.</p>
<p>However, revocation of the issued verifiable document will require the
setup of document store and hence will incur gas fee. Please refer to
<a href="https://docs.tradetrust.io/docs/advanced/aws-kms/did-sign-demo" rel="noopener noreferrer nofollow" target="_blank">https://docs.tradetrust.io/docs/advanced/aws-kms/did-sign-demo</a>for
more details.</p>
<p>&lt;&lt;&gt;&gt;&gt;&gt;&gt;</p>
<p>The DID is currently only applicable for normal/verifiable documents.
By using the DID approach, the issuance of normal/verifiable documents
will not incur any gas fee.</p>
<p>However, revocation of the issued docs will require the setup of document
store and hence will incur gas fee. See <a href="https://docs.tradetrust.io/docs/advanced/aws-kms/did-sign-demo" rel="noopener noreferrer nofollow" target="_blank">DID approach detail.</a>
</p>