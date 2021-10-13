# Installing Matomo on your wordpress

You can use the same tracking code for your platform site and your wordpress site.\
\
1\. Once you have Matomo set up, add the Matomo plug-in to your wordpress page: [https://wordpress.org/plugins/wp-piwik/#description](https://wordpress.org/plugins/wp-piwik/#description)

2\. Then go to your wordpress admin page /wp-admin/options-general.php?page=wp-piwik%2Fclasses%2FWP_Piwik.php (e.g.[https://about.openfoodnetwork.org.au/wp-admin/options-general.php?page=wp-piwik%2Fclasses%2FWP_Piwik.php](https://about.openfoodnetwork.org.au/wp-admin/options-general.php?page=wp-piwik%2Fclasses%2FWP_Piwik.php) )

3\. Select Innocraft cloud hosted Matomo

4\. Add openfoodnetwork as the Innocraft subdomain

5\. Enter your auth token - To get your auth token, log in to Matomo, click at the preferences gear icon (top right) and click at “API” (left sidebar menu, near the bottom). You can get a more detailed description here: https://matomo.org/blog/2015/05/wordpress-integration-wp-piwik-1-0/

6\. Uncheck the box that says Auto config

7\. Select which site you're tracking (e.g. OFN Australia)

