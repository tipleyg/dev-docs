# Channel App Requirements

<!-- Dev Center URL: https://developer.bigcommerce.com/api-docs/channels/guide/channel-app-requirements -->

Once approved, channel apps are discoverable on BigCommerce's App Marketplace. Additionally, apps developed by [select partners](https://www.bigcommerce.com/partners/) are marketed in the Channel Manager within the Control Panel of every store. To be approved, channel apps must meet certain requirements. This article lists the requirements for publishing channel apps to both locations.

## General requirements

All Partners:

- Uses [Channels API](https://developer.bigcommerce.com/api-reference/cart-checkout/channels-listings-api).

- [Creates a channel](https://developer.bigcommerce.com/api-reference/cart-checkout/channels-listings-api/channels/createchannel) upon app installation.
- Reads and updates channel status using the [Channels API](https://developer.bigcommerce.com/api-reference/cart-checkout/channels-listings-api) endpoints.

- Follows requirements for specific channel type

- Contains an onboarding user flow

Select Partners:

- Uses [Big Design](https://developer.bigcommerce.com/big-design/).

- Includes `config_meta.app.id` in the [create channel](https://developer.bigcommerce.com/api-reference/cart-checkout/channels-listings-api/channels/createchannel) request.

<div class="HubBlock--callout">
<div class="CalloutBlock--info">
<div class="HubBlock-content">

> ### Note
>
> - You can find the app ID in the URL when editing the app in the [Developer Portal](https://devtools.bigcommerce.com/). For more information, see [Finding an App's ID](https://developer.bigcommerce.com/api-docs/apps/tutorials/id).
> - `config_meta.app.id` is optional; however, if you're building an app that creates or manages a channel, we recommend including the app ID to ensure the user interface in the BigCommerce control panel works properly.
> - Select partners who are promoted in the Channel Manager must build an app, and include the app ID in the create channel request.

</div>
</div>
</div>


## Storefronts

All Partners:

- Must use [Sites and Routes API](https://developer.bigcommerce.com/api-reference/cart-checkout/sites-routes-api) so that links generated within BigCommerce, such as "view storefront" and links sent in transactional emails to shoppers, will use the headless storefront's correct URL.

## Marketplaces and marketing

All Partners:

- Must use [Listings API](https://developer.bigcommerce.com/api-reference/cart-checkout/channels-listings-api), if supporting per product listings.

<div class="HubBlock--callout">
<div class="CalloutBlock--info">
<div class="HubBlock-content">

<!-- theme: info -->

> **Note**
>
> - In order to promote app performance and user experience best practices, additional general and channel type requirements will be outlined as needed.

</div>
</div>
</div>

## Related resources

### Articles

- [Channels Overview](https://developer.bigcommerce.com/api-docs/channels/overview)
- [Building Channel Apps](https://developer.bigcommerce.com/api-docs/channels/building-channel-apps)
- [Becoming a Partner](https://developer.bigcommerce.com/api-docs/partner/becoming-a-partner)
- [Types of Apps](https://developer.bigcommerce.com/api-docs/getting-started/building-apps-bigcommerce/types-of-apps)
- [Authenticating BigCommerce's REST APIs](https://developer.bigcommerce.com/api-docs/getting-started/authentication/rest-api-authentication)
- [Building an App](https://developer.bigcommerce.com/api-docs/getting-started/building-apps-bigcommerce/building-apps)
- [App Store Approval Requirements](https://developer.bigcommerce.com/api-docs/partner/app-store-approval-requirements)

### Endpoints

- [Channels API Reference](https://developer.bigcommerce.com/api-reference/cart-checkout/channels-listings-api)
- [Sites and Rites API Reference](https://developer.bigcommerce.com/api-reference/cart-checkout/sites-routes-api)
