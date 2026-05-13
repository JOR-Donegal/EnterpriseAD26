# Introduction

!!! abstract "Enterprise AD"

For any non-trivial site, we need to centralize AAA. We previously did this by setting up an Active Directory domain. Even on the simplest of sites, we need two domain controllers per domain, and we ensure we have a backup and recovery plan before the site goes live. And in fact, this simple approach probably represents 99% of all sites. The entire Letterkenny campus of ATU is a single domain. If we define Active Directory as an administrative boundary, that's a good place to start. As a single domain it's also a security boundary.

Most environments you work with will have a single domain. In most cases, there is one technical group looking after the organization. However, in large and complex organizations, we may need additional administrative boundaries. Suppose we are planning a large and complex multinational organization. Policy may be controlled centrally by the corporate headquarters.

Technical support is done locally in each jurisdiction; the technicians in each country need full control of their domain. And we may need to provide access to the resources in a local domain, to users from another location who do not have accounts in that domain.

In fact, any user in any local organization, may be required to work at another site.

It is in these larger scenarios that AD is the platform of choice for most of us.
