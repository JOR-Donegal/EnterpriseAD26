# Hierarchical namespace

We address issues like this by building a complex domain structure. One example would be a single organization, with multiple sites which we need administered locally. At corporate headquarters, we build a root domain, this is the first domain in a new _Forest_. For example, electric-petrol.ie. At each local site which needs to be independently administered, I create a child domain; for example, _buncrana.electric-petrol.ie_ and _letterkenny.electric-petrol.ie._ Each child domain can assign administrators to the domain administrator’s group and have full local control. There is a group in the root domain called enterprise administrators who have control over the root and all child domains.

<figure>
<img src = "https://jor-donegal.github.io/EnterpriseAD26/images/fig1.png">
<figcaption>Fig 1. Tree.</figcaption>
</figure>

When we created domain tree like this, there is an implicit trust relationship between the domains; this is what the blue lines indicate. A user account in the Buncrana domain can be assigned privileges in the Letterkenny domain. When you add a child domain, a _two-way transitive trust_ is added by default; if 1 trusts 2 and 1 trusts 3, then 2 trusts 3.

Note that all these domains are in the same hierarchical namespace; they are all part of the root _electric-petrol.ie_ and this is the easiest case to consider.

