# Nomenclature

Let me start off with some terminology and definitions.

In a _domain_, we can have a domain admins group, and if you are a member of that group, you have control of most aspects of the domain. Just for completeness, there are permissions like _schema admin_, which a domain admin does not have. 

For this reason, we will give a final definition of a domain as being an __administrative boundary__.

When we have a large organization, we may have some more complex design requirements.

1. The large organization may have multiple administered domains all organized in a coherent manner.
2. The organization will have policy control which is centralized and overriding.
3. Any user on any site, may be given access permissions to any other domain. Users then are normally members of global groups.
4. Resources on any sites our grouped, by means of site local groups.
5. Access permissions a granted by giving a global user group membership of a site local group associated with a resource.

Complicated!
