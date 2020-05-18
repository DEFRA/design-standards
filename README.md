
# Defra design Standards

The Department for Environment, Food & Rural Affairs (Defra) are the UK government department responsible for safeguarding our natural environment, supporting our world-leading food and farming industry, and sustaining a thriving rural economy. 

Defra services are designed to meet user needs and to protect the environment.


All Defra's online services must:

-   Be designed to meet the Government [service standard](https://www.gov.uk/service-manual/service-standard)

-   Meet the [government accessibility requirements](https://www.gov.uk/service-manual/helping-people-to-use-your-service/making-your-service-accessible-an-introduction#meeting-government-accessibility-requirements)

-   Be designed based on user needs

* * * * *

Contents:

-   [Defra design standards](#design-standards)
-   [Non gov.uk domains](#non-govuk-domains)
-   [cookies and similar technologies](#cookies-and-similar-technologies)
-   [Inclusive design](#inclusive-design)
-   [accessibility](#accessibility)
-   [maps](#maps)
-   [data and charts](#data-visualisation)
-   [internal services](#internal-services)
-   [components & patterns](#components-and-patterns)

* * * * *


## Non GOV.uk domains

Services and websites hosted on non GOV.uk domain names must still meet the Government [service standard](https://www.gov.uk/service-manual/service-standard).

All public-facing services should look and feel like part of GOV.UK, so users know they're in the right place.

Non GOV.uk domains should:

-   not use the 'New Transport' font
-   not use the GOV.uk Header or crown logo
-   not use the GOV.uk footer

### Font

Use the Helvetica or Arial CSS font stacks.

### Colour

Colors should be consistent with the [GOV.UK front end kit](https://design-system.service.gov.uk/styles/colour/). 

Agency or department colours can be used sparingly for example in headers or navigation.

You must make sure that the contrast ratio of text and interactive elements in
your service meets [level AA of the Web Content Accessibility Guidelines (WCAG 2.1)](https://www.w3.org/TR/WCAG21/#contrast-minimum).

| Department         |          |                    |                       |
|--------------------|----------|--------------------|-----------------------|
| Defra              | \#00a33b | rgb\(0, 163, 59\)  | hsl\(142, 100%, 32%\) |
| Environment Agency | \#009E43 | rgb\(0, 158, 67\)  | hsl\(145, 100%, 31%\) |
| Natural England    | \#00AB52 | rgb\(0, 173, 84\)  | hsl\(149, 100%, 34%\) |
| APHA               | \#00a33b | rgb\(0, 163, 59\)  | hsl\(142, 100%, 32%\) |
| MMO                | \#00a33b | rgb\(0, 163, 59\)  | hsl\(142, 100%, 32%\) |
| RPA                | \#00a33b | rgb\(0, 163, 59\)  | hsl\(142, 100%, 32%\) |

### Header and Footer

Defra or supporting agency page templates should be used in place of the GOV.uk templates for:

-   Internal facing services (case management systems, intranets etc)
-   External facing services not hosted on GOV.uk

![Defra header](/img/main-header.png)
*Example Defra header*

![Defra header version 2](/img/small-header.png)
*Example Defra header*

### Logo

For external facing sites not on Gov.uk a Defra or supporting agency logo must be used.

Organisation logos must be included as an SVG where possible. The crest image itself must be presentational and ignored by screen readers.

Links in the logo must:

-   accept focus
-   be focusable with a keyboard
-   be usable with a keyboard
-   indicate when they have focus
-   change in appearance when touched (in the touch-down state)
-   change in appearance when hovered
-   be usable with touch
-   be usable with [voice commands](https://www.w3.org/WAI/perspectives/voice.html)
-   have visible text
-   have meaningful text

[View the organisation logo component](https://components.publishing.service.gov.uk/component-guide/organisation_logo)

[View the component CSS](https://github.com/alphagov/govuk_publishing_components/blob/master/app/assets/stylesheets/govuk_publishing_components/components/_organisation-logo.scss)

-------------

## Cookies and similar technologies

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

[Read the full compliance guidance document](/Cookies-and-similar-technologies.md)

-------------

## Inclusive design

All Defra services should be designed to be inclusive. Inclusive design aims to remove the barriers that create undue effort and separation.

It enables everyone to participate equally, confidently and independently in everyday activities.

Principles of inclusive design:

-   Inclusive -- so everyone can use it safely, easily and with dignity
-   Responsive -- taking account of what people say they need and want
-   Flexible -- so different people can use it in different ways
-   Convenient -- so everyone can use it without too much effort or separation
-   Accommodating for all people, regardless of their age, gender, mobility, ethnicity or circumstances
-   Welcoming -- with no disabling barriers that might exclude some people
-   Realistic -- offering more than one solution to help balance everyone's needs and recognising that one solution may not work for all

-------------

## Accessibility

Making a website or mobile app accessible means making sure it can be used by everyone, including those with:

-   impaired vision
-   motor difficulties
-   cognitive impairments or learning disabilities
-   deafness or impaired hearing

Public Sector Body Accessibility Regulations 2018 became UK law in September 2018 meaning public sector organisations have a legal duty to make sure websites and apps meet accessibility requirements.

To meet accessibility requirements, digital services must:

-   meet level AA of the  [Web Content Accessibility Guidelines (known as WCAG 2.1)](https://www.gov.uk/service-manual/helping-people-to-use-your-service/understanding-wcag-20)  as a minimum
-   work on the most commonly used [assistive technologies](https://www.gov.uk/service-manual/technology/testing-with-assistive-technologies) -- including screen magnifiers, screen readers and speech recognition tools
-   include people with disabilities in [user research](https://www.gov.uk/service-manual/user-research/running-research-sessions-with-people-with-disabilities)
-   publish an accessibility statement that explains how accessible your website or mobile app is

### WCAG standards

WCAG stands for Web Content Accessibility Guidelines and is the standard by which accessibility is measured regardless of whether the digital service is a website, product or app.

WCAG 2.1 is an extension to WCAG 2.0. It breaks down into four sections:

-   Perceivable - Information is presented in ways that can be accessed by everyone
-   Operable - Information is presented in ways that can be operated by everyone
-   Understandable - Information is presented in ways that can be understood by everyone
-   Robust - Information is reliable and compatible with assistive technology and standards

Not all accessibility issues can be detected automatically. Manual testing is always required.

[View the Defra accessibility checklist](https://drive.google.com/file/d/1I9l_ImXjJMpR3tZY-1lN63Rub6SK2tdq/view?usp=sharing)[ ](https://www.gov.uk/government/publications/sample-accessibility-statement/sample-accessibility-statement-for-a-fictional-public-sector-website#technical-information-about-this-websites-accessibility)

### Accessibility statements

All public sector websites will need to publish an accessibility statement. The accessibility statement should:

-   list any inaccessible parts of the website or app
-   show how people with access needs can get alternatives to content that's not accessible
-   provide details on who to contact to report accessibility issues
-   provide information on the enforcement procedure if people are not happy with the response
-   be published in a fully accessible form
-   follow a consistent format

[View a sample accessibility statement](https://www.gov.uk/government/publications/sample-accessibility-statement/sample-accessibility-statement-for-a-fictional-public-sector-website#technical-information-about-this-websites-accessibility)

-------------

## Maps 

All essential geographic information must be available in non visual formats such as text or lists.

Maps should be used as visual enhancements of this information for people who choose to use them.

Interactive maps should only be used when there is a user need.

[Read the full guidance on working with maps](/Maps.md)

-------------

## Data visualisation


All essential data and information must be available in non visual formats such as text or lists.

Charts and graphs should be used as visual enhancements of this information for people who chose to use them.

<!-- Read the full guidance on working with maps (coming soon) -->

-------------

## Internal services

Internal facing services and case management tools need to be consistent across Defra.

Standardisation increases usability and familiarity making sure systems are efficient, easy to use and accessible. 

### Procurement

Any products bought from external suppliers need to meet the [Technology code of practice](https://www.gov.uk/government/publications/technology-code-of-practice/technology-code-of-practice)

<!-- Read the full guidance on case management systems (coming soon) -->

-------------

## Components and patterns

Design patterns solve the common problems so teams can focus on the things unique to their service and it's users.

Check the [GOV.UK Design System](https://design-system.service.gov.uk/) to see if the component or pattern you need is already being used across government.

If you cannot find what you need in the GOV.UK Design System you can:

1.  [see if it is being worked on by other teams across government ](https://design-system.service.gov.uk/community/backlog/)and add your findings

2.  [see if it is being worked on by someone in Defra](https://github.com/DEFRA/design-discussions/issues) and add your findings

3.  Check other departments for [design patterns and design resources](https://github.com/ctdesign/gov-design-systems-list)

4.  [propose a new pattern in the Defra backlog](https://github.com/DEFRA/design-discussions/issues)

5.  [propose a new pattern in the GOV.UK Design System](https://design-system.service.gov.uk/community/propose-a-component-or-pattern/)

All patterns must be [useful and unique](https://design-system.service.gov.uk/community/contribution-criteria/#new-proposals).

### Iterating a component or pattern

Existing design patterns can be used as starting points but may need to be iterated to suit the needs of users of a particular service.

Before iterating a component or pattern make sure there is a clear user need to do so. Share any changes you make or research findings to the [GOV.UK design system backlog](https://github.com/alphagov/govuk-design-system-backlog/issues).

To do this add a class to the component with a Defra namespace.

#### Default

```

<button type="submit" class="govuk-button">

  Save and continue

</button>

```

#### New

```

<button type="submit" class="govuk-button defra-button">

  Save and continue

</button>

```

### New components

To create a new pattern use a Defra namespace to avoid issues with CSS inheritance.

```

<header role="banner" class="defra-internal-header">

   <div class="defra-logo">

       <a href="#" title="#" class="defra-logo__link">

           <span class="c-defra-logo__title"> Logo text</span>

       </a>

   </div>

   <div class="defra-internal-service-name">

       <a href="/" title="Go to the homepage" class="defra-internal-service-name__link">

         Internal service name

       </a>

   </div>

</header>

```