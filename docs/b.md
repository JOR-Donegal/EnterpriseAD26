# Hierarchical namespace

We address issues like this by building a complex domain structure. One example would be a single organization, with multiple sites which we need administered locally. At corporate headquarters, we build a root domain, this is the first domain in a new Forest. For example, electric-petrol.ie. At each local site which needs to be independently administered, I create a child domain; for example, _buncrana.electric-petrol.ie_ and _letterkenny.electric-petrol.ie._ Each child domain can assign administrators to the domain administrator’s group and have full local control. There is a group in the root domain called enterprise administrators who have control over the root and all child domains.

<figure>
<img src = "https://jor-donegal.github.io/EnterpriseAD26/images/fig1.jpg">
<figcaption>Fig 1. Tree.</figcaption>
</figure>