# Piwik Pro GTM server-side with ecommerce-events (GA4-based)
A tag template for Piwik Pro server-side tracking inside Google Tag Manager with full support of popular ecommerce events based on the default Google Analytics 4 implementation specifications.

## How to implement the tag
1. Go to your Google Tag Manager server-side container
2. Import the [tag template file](https://github.com/endgameapp/piwikpro-gtm-serverside/blob/main/piwikpro-gtm-serverside-ga4.tpl) in this repo at: Templates -> Tagtemplates -> New -> Import (under ... in top right menu)
3. Save the tag template
4. Go to Tags -> New -> Piwik Pro server-side (GA4-based)
5. Configure the tag
6. Choose a custom trigger with: Client Name = GA4
7. Test & Publish your server-side container
8. Sit back & relax, let the revenue come in (allow for a small delay in processing the data)

## How to configure the tag
Coming soon...

## Supported GA4 events
1. page_view: generic page view events
2. purchase: ecommerce transactions

## More resources
1. [Piwik Pro HTTP API](https://developers.piwik.pro/en/latest/data_collection/api/http_api.html)
2. [Piwik Pro ecommerce tracking](https://help.piwik.pro/support/getting-started/track-ecommerce/)
3. [Default Google Anayltics 4 events](https://developers.google.com/analytics/devguides/collection/ga4/reference/events)
4. [A complete guide to server-side tagging](https://www.simoahava.com/analytics/server-side-tagging-google-tag-manager/)

## Support with server-side tagging
In case you need professional help with setting up server-side tagging inside Google Tag Manager you can [contact me here](https://dennisvreeke.com).
