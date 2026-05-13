# Multiple Forests

It may be that the legal reasons, for audit purposes, or due to organizational structures, that we do not want anything like the enterprise administrator’s group. In this case we may have separate forests.

<figure>
<img src = "https://jor-donegal.github.io/EnterpriseAD26/images/fig3.png">
<figcaption>Fig 3. Multiple forests.</figcaption>
</figure>

There is no trust relationship between the forests; if you need to create one, you need to create a manual trust.

Trust relationships are created automatically most of the time. _Two-way transitive trusts_ can pass through an entire forest, regardless how complex. All domains in a forest trust all domains in a forest.

If you have a second forest, there is no automatic, two-way trust between forests. The Domains and Trusts MMC snap-in gives us access to see trusts. Note that the trusting and being trusted are separate! I could configure the solar-sweets.net to trust electric-petrol.ie but not set up the trust for electric-petrol.ie to solar-sweets.net; this is a one-way trust between domains.
