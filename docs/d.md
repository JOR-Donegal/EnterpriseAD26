# Greenfield

In the first half of my teaching modules, the scenario is that we're working on a Greenfield site, the size of an SME, and with no Internet connectivity. In all of these cases the domain name almost doesn't matter. But let's do it properly anyway!

The organization name is electric petrol, and the registered domain name is _electric-petrol.ie_ for the entire organization. 

For the second 6 weeks, things get more complex.

When you register a fully qualified domain name, that is your domain for the Internet. The only DNS records which should exist for that domain are the ones for public services and necessary housekeeping.

For example

- ns1.electric-petrol.ie
- ns2.electric-petrol.ie
- ftp1.electric-petrol.ie
- www1.electric-petrol.ie

Your internal services should not be in the same domain or namespace! We need a _delegation_ from the top level to a _sub-domain_...or maybe no connection at all? This is called _split-brain DNS_.

If I were setting up a single site in Buncrana, I would most likely call it _buncrana.electric-petrol.ie_ but that is lazy!

In a large organization there may be more than one sub-domain and they may not all be AD. Best practice for a large organization is to pick a name for the top level AD. In the second 6 weeks of my modules, the scenario is for a single centralized organization with >60 sites, interconnected.So the first domain in this scenario is _ads.electric-petrol.ie_

I create this domain as the top of the hierarchy that holds the organization together. I will create at least two DCs, in separate data centers.

I will create a domain for Buncrana as a child domain to ads.electric-petrol.ie, as _buncrana.ads.electric-petrol.ie_

The end result will be a top level internal domain and c. 60 child domains.