# Numbers format

Each country has its own convention on how numbers are displayed and use various separators for thousands and decimals.

To make it easier we have implemented the following internationalization logic:
- Whatever the way the number is filled in, it is interpreted, translated and displayed in the default Spree format which is "No thousands separator + a dot (.) for decimal separators."
- So that means that if you enter "3,50" as a price that will be translated and displayed "3.50", "3" will become "3.00", "3.500" will become "3500.00" and  "3,500" will become "3500.00" (we consider that a price can't have 3 decimals and interpret that as , or . being the thousands separator).
- So this logic is supposed to cover any case of numbers format internationally. If you think your case doesn't fit in while testing please reach out.

[one thing still mysterious to me, before the last Spree upgrade we had set up the French instance to display decimals with , which is still the case in shopfront but the configuration panel for that has disappear...]

To use that internationalization logic go to **Configuration > General settings** and look for "Number localization settings"
You will see a checkbox proposing you to "use the international thousand/decimal separator logic".
![](/assets/Screenshot from 2018-04-02 11-22-11.png)