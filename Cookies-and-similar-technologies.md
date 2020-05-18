# Cookies and similar technologies

To comply with the The Privacy and Electronic Communications Regulations (PECR) you must:

-   tell people if your site uses cookies or similar technologies

-   clearly explain what the cookies do and why

-   not store cookies for longer than is necessary  

-   get a user's explicit consent before storing or retrieving non-essential cookies on their device

-   save a user's consent preferences for 1 year only

-   not store any unique identifiers in the consent preferences cookie

A user must be able to:

-   withdraw consent as easily as they give it

-   make changes to their cookie settings

-   use the service without consenting to the use of cookies 

![Cookie consent flow diagram](/img/consent-flow.jpg)
*Cookie consent flow diagram*

## Similar Technologies

The same rules also apply if you use any other type of technology to store or gain access to information on someone's device.

Other technology examples:

-   Fingerprinting

-   HTML5 web storage API

-   IndexedDB API

## Cookie banner

The user must be clear that by taking an action they are giving consent for you to store cookies on their computer or device.

A cookie banner must not attempt to influence a user's decision.

View the [Cookie banner component](https://components.publishing.service.gov.uk/component-guide/cookie_banner)

View the [page template which pulls in the banners](https://github.com/alphagov/static/blob/54706a6eddcf71e2d6cd36b3239798293530d4e6/app/views/layouts/govuk_template.html.erb#L50).

## Notification banner

The user must be notified that their chosen settings have been saved. The banner should link to the cookie settings page.

## Cookie settings

The settings page must be linked to from the footer allowing users to easily update their preferences.

Radio buttons should be set to "Do not use cookies that measure my website use" until consent is gained.

![cookie settings page](/img/cookie-settings.png)
*Cookie settings page example*

[View an example cookie settings page](https://www.gov.uk/help/cookies)

## Cookie details

The cookie detail page must clearly explain what cookies do and why they are being used.

The user must have clear information on all the cookies used including:

-   the cookie name

-   the purpose of the cookie

-   when the cookie will expire

The details page must have a clear link to the cookie settings page.

[View an example cookie details page](https://www.gov.uk/help/cookie-details)

## Essential or strictly-necessary cookies

Essential cookies can be used without gaining consent. An essential cookie does not store personal data and is removed once the interaction is complete.

Essential cookies can be used to: 

-   save a user's progress through an online form

-   ensure the security of a user's data

-   distribute load across a number of servers

Users must still be notified of the cookie's existence with a notification banner.

Users must still be able to find out more information on the cookies used in a cookie information page.

Essential cookies should expire as soon as possible, without impacting the user experience. This could be when a user completes their journey or a set time of 2-4 hours.

The expiry time may be reset each time a user interacts with the service, for example moving to the next screen of a journey.

![Notification banner](/img/notification-banner.jpg)
*Essential cookies notification banner*

![essential cookies flow](/img/essential-cookies.jpg)
*Essential cookies flow diagram*

## Security

All Defra services should:

-   only use first-party cookies

-   not store sensitive information inside a cookie, cookies should store a unique identifier which can be used to retrieve sensitive information from a server-side database/ca

## Cookie settings

-   set the 'Secure' flag on cookies - a secure cookie is only sent to the server with an encrypted request over the HTTPS protocol.  This helps to mitigate session hijacking through man in the middle attacks.

-   set the 'HttpOnly' flag on cookies - to help mitigate cross-site scripting (XSS) attacks, HttpOnly cookies are inaccessible to JavaScript's Document.cookie API; they are only sent to the server

-   set the 'SameSite' property to 'Strict' - in strict mode, the browser will only send cookies for same-site requests (requests originating from the site that set the cookie)

-   use the '__Host-' prefix for sensitive cookies (e.g. session cookies) when setting the name of the cookie. Read more about[ the _Host- prefix](https://developer.mozilla.org/en-US/docs/Web/HTTP/Cookies#Cookie_prefixes).