# UPN Suffixes

We have seen that there are two types of login name;

1. Modern: john.oraw@letterkenny.lyit-cdc.net
2. Pre-Windows 2000: Letterkenny\john.oraw

With the modern names, they can get long and cumbersome. We call the full path a _UPN suffix_. We can create additional _User Principal Name_ (UPN) suffixes and we almost always do this to simplify things.

Note that these suffixes are forest wide, we must be careful to ensure usernames are unique forest wide. In the Domain and Trusts tool, I can create alternate suffixes.

<figure>
<img src = "https://jor-donegal.github.io/EnterpriseAD26/images/fig4.png">
<figcaption>Fig 4. UPN Suffixes.</figcaption>
</figure>

For each user, I can select which suffix to use. As long as the usernames are unique, I can keep all users on simple suffixes, regardless of how long their local domain name is!

<figure>
<img src = "https://jor-donegal.github.io/EnterpriseAD26/images/fig5.png">
<figcaption>Fig 5. Customizing.</figcaption>
</figure>





