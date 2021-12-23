---
description: How to plug Matomo to your instance in order to measure users behaviour.
---

# Matomo settings

[Matomo ](https://matomo.org)is the analytics tool that we have chosen to implement within OFN as it is fully [GDPR](https://eugdpr.org) compliant. OFN has a global Matomo account. Just ask on Slack on instance managers channel for someone to give you access to this global account.

As a superadmin, here is what you see in the configuration "Matomo Settings" tab:

![](../../.gitbook/assets/matomo-config-screen.png)

**Matomo URL:** Fill in the following URL [https://openfoodnetwork.innocraft.cloud/](https://openfoodnetwork.innocraft.cloud)  &#x20;

{% hint style="info" %}
**Do not delete the "/" at the end of the URL otherwise it's not working! The URL is the same for ALL instances**
{% endhint %}

**Matomo Site ID:**  The image below shows where to find this number in the global Matomo account.

![](https://lh6.googleusercontent.com/mKWjaq9Z4Rr3UOPD3CTA2IQYt4KJWo4QcoloG1h5UOR4uCKUcLzhWeqjKTKTeEm7YO9D7d\_3VxA0IPA53aw4sj0ZQZvEmnvWxY-D0o68culnfurAmfgma7BqqyMGQjcfE0Zs-Qsd)

If you don't see your instance in the list, you will have to [create a new Matomo site](setting-up-a-new-matomo-site.md).&#x20;

**Matomo Tag Manager URL:** The tag manager allows you to set up events for very specific user interactions. Navigate to your tag manager via the main menu:

![](../../.gitbook/assets/matomo-nav.png)

The Matomo Tag Manager URL is copied from the Install Code section of Matomo Tag Manager. Ensure you select the right container and environment as these options change the URL.

![](<../../.gitbook/assets/Screen Shot 2020-07-01 at 2.05.18 pm.png>)

The URL should look something like this, your container ID (eg abc123xyz) will be different:\
https://cdn.innocraft.cloud/openfoodnetwork.innocraft.cloud/container\_**abc123xyz**.js\
\
Select update after entering all the settings and that's it, the Matomo tracking code will now be embedded in pages on your OFN instance.

Lastly if you are using Matomo, you will want to notify your users. Do this by selecting "**Display Matomo section on cookies policy page**" in [Configuration > General Settings](https://ofn-user-guide.gitbook.io/ofn-super-admin-guide/ofn-platform-configuration/general-settings).

![](<../../.gitbook/assets/image (4).png>)



