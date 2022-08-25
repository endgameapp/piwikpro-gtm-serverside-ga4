# Piwik Pro GTM server-side with ecommerce-events (GA4-based)
A tag template for Piwik Pro server-side tracking inside Google Tag Manager with full support of popular ecommerce events based on the default Google Analytics 4 implementation specifications. 

Note: this template is specifically for Google Analytics 4 clients. The repository of Piwik Pro server-side template based on Universal Analytics is located [here](https://github.com/PiwikPRO/server-side-template-for-gtm).

## How to implement the tag
We assume that you already have enough knowledge about server-side Google Tag Manager to implement the tag. Below you can find the steps to enable this template inside your container.
1. Go to your Google Tag Manager server-side container
2. Import the [tag template file](https://github.com/endgameapp/piwikpro-gtm-serverside/blob/main/piwikpro-gtm-serverside-ga4.tpl) in this repo at: Templates -> Tagtemplates -> New -> Import (under ... in top right menu)
3. Save the tag template
4. Go to Tags -> New -> Piwik Pro server-side (GA4-based)
5. Configure the tag
6. Choose a custom trigger with: Client Name = GA4
7. Save, test & publish your server-side container
8. Sit back & relax, let the revenue come in (allow for a small delay in processing the data)

## Default GA4 events
We have mapped the following default GA4 events (based on [this](https://developers.google.com/analytics/devguides/collection/ga4/reference/events) and [this](https://support.google.com/analytics/answer/9234069?hl=en&ref_topic=9756175) list) to the format of Piwik Pro. All other events will be considered custom Piwik Pro events and can be mapped with the values you prefer. 
1. page_view: generic page view events
2. purchase: ecommerce transactions
3. scroll: scroll depth of the page
4. user_engagement: user engagement time in seconds
5. click: outbound link clicks
6. file_download: registering file downloads
7. add_payment_info: when a user chooses a payment method
8. add_shipping_info: when a user chooses a shipping method
9. login: when a user logins in the application
10. sign_up: when a user signups
11. share: social shares

## Custom events (all your remaining GA4 events)
Additionally, you can use the mapping settings inside the tag settings to provide Piwik with the right Event Category, Action and Value. If the GA4 event is not mapped but still send to Piwik Pro, then it will get listed under Event Category 'ga4_events' with the event name set as Event Action.
1. Enable the 'Custom event mapping' setting
2. Provide the Google Analytics 4 event name in the first column
3. Enter columns Event Categy (required), Action (required), Value (optional) in plain text or choose a variable (e.g. event data)
4. Save, test & publish your server-side container

## Excluding events from Piwik Pro
Coming soon...

## More resources
1. [Piwik Pro HTTP API](https://developers.piwik.pro/en/latest/data_collection/api/http_api.html)
2. [Piwik Pro ecommerce tracking](https://help.piwik.pro/support/getting-started/track-ecommerce/)
3. [GA4 default events](https://developers.google.com/analytics/devguides/collection/ga4/reference/events)
4. [GA4 automatically collected events](https://support.google.com/analytics/answer/9234069?hl=en&ref_topic=9756175)
5. [A complete guide to server-side tagging](https://www.simoahava.com/analytics/server-side-tagging-google-tag-manager/)

## TODO list
Coming soon...

## Support with server-side tagging
In case you need professional help with setting up server-side tagging inside Google Tag Manager you can [contact me here](https://dennisvreeke.com).
