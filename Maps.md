# Defra map design Standards

If a map is used to provide visual enhancements to existing information it must be designed and built inclusively.

* * * * *

Contents:

-   [before you start](#before-you-start)
-   [prototyping](#prototyping)
-   [colour](#colour)
-   [keyboard](#keyboard)
-   [Mobile](#mobile)
-   [Interactive elements](#interactive-elements)
-   [mark up](#mark-up)
-   [progresive enhancement](#progresive-enhancement)

* * * * *

## Before you start

Before you start designing a map you must:

-   Carry out user research without a map to find out if one is needed

-   Consider the digital and spatial-data literacy of your users

If you users do need a map you need to determine if the map needs to be:

-   Static

-   Interactive (zoom, layers, key etc)

-   User driven (shape tools, selecting areas etc)Level 3 - draw shapes etc?

All maps should:

-   Be as simple as possible

-   Use vectors not static image formats

-------------

## Prototyping

Interactive elements need to be tested early with users using prototypes.

Prototyping tools:

-   [Google maps](https://www.google.co.uk/maps/about/mymaps/)

-   [Map box](https://docs.mapbox.com/playground/static/)

-   [geojson](http://geojson.io/#map=2/20.0/0.0)

-   [Mapstarter](http://mapstarter.com/)

-------------

## Colour

Colour alone should not be used to convey meaning.

When working with colours you should:

-   Check colour contrasts meet WCAG standards

-   Check the colour combinations work in greyscale

-   Check colours work in high contrast and dark modes

-   Check colours work for people with colour vision deficiency (color blindness)

-   Consider adding patterns so that colours are distinguishable to people with colour vision deficiency 

-   Consider semantic meaning of colours (e.g. are users used to a certain colour meaning something for maps on this topic?)

-   Directly labelling features can help to make sure maps don't rely on colour

-   Design feature icons that are unique and don't rely on colour

-------------

## Keyboard

The same functionality should be provided to keyboard users as to mouse, touch and audio users.

A user needs to:

-   Be able to tab through map in a logical reading order

-   Be able to skip maps completely by tabbing through a page

-   Be able to navigate a maps components and interact using a keyboard

-   Have clear signposting using focus styles

-------------

##mMobile/Touch

In May 2020 59% of all government website traffic was on mobile. [View the latest Government device statistics](https://www.gov.uk/performance/site-activity/device-type).

All map components must work and be understood on:

-   A [range of browsers and devices](https://www.gov.uk/service-manual/technology/designing-for-different-browsers-and-devices#browsers-to-test-in) 

-   Small screen sizes

-   Devices with touch interfaces

Optimise limited screen space by using modal windows for contextual information

All interactive elements of the map must be operable using touch interface only.

All map components must:

-   Use standard touch patterns such as pinch, zoom and drag pan.

-   Have a large hit area for controls (minimum of 40px square)

For complex interactive maps consider designing a [progressive Web App (PWA)](https://technology.blog.gov.uk/2018/03/26/progressive-web-apps-bring-us-new-mobile-opportunities/).

-------------

## Interactive elements

Interactive maps allow users to control what they see using keys, labels, points, polygons and polylines.

Interactive elements should only be used where there is a clear user need. Don't make designs too intricate otherwise people with motor and physical disabilities will struggle.

All interactive elements of the map must be operable using a keyboard or a mouse

All interactive elements should:

-   Have clear affordances so that's obvious to all users that they are interactive

-   Have hover and focus styles that are consistent with the rest of the service

-   Reveal contextual information using dialogue boxes

### Keys and legends

Where possible a key should use dynamic data, only describing features that are currently being displayed on the map.

-------------

## Mark up

Depending on the nature of the map there are different approaches to markup. 

### Static

<figure>

    <figcaption>

        <h2>Map title</h2>

        <p>Map description</p>

    </figcaption>

    <div>

        ...Map stuff here...

    </div>

    <footer>

        <a>Download data</a>

        <p>Other small print</p>

    </footer>

</figure>

### Interactive (zoom, layers, key etc)

<figure>

    <figcaption>

        <h2>Map title</h2>

        <p>Map description</p>

    </figcaption>

    <div>

        ...Map stuff here...

    </div>

    <footer>

        <a>Download data</a>

        <p>Other small print</p>

    </footer>

</figure>

### User driven (shape tools, selecting areas etc)

Application

Things to consider:

-   Consider page title when map is fullscreen

-   Consider role of 'application' if complex and has bespoke interactions

-   Consider the experience for screen reader users. Ie if they can't get any value from the map then ensure there are no screen reader traps and they are directed to the accessible content.

-   Nested dialogs both modal and non-modal

-   Desktop vs mobile modal/non-modal behavior may be different?

-   Provide fallback content within the canvas element

-------------

## Progressive enhancement

Progressive enhancement is a strategy for web design that emphasizes core webpage content first.

Map components should follow the same principle.

-   Core content should be available without JavaScript, or the map fails to load

-   Core content should also be available via another accessible routes (e.g. a nearby data table or spreadsheet download)

It may be impossible to make the interactive map accessible to assistive technology like screen readers, if this is the case consider hiding it with `aria-hidden="true"`

-------------

## Background mapping/tiles

Background maps contain general geographic information like place names, roads and natural features. They give useful visual context to the interactive features that we layer on top.

-   Turn off any background layers you don't need (e.g. hide roads if roads aren't important to your users)

-   Make sure the text on background tiles legible (e.g. increase size and contrast of labels)

-   Choose colours and font styles that match the rest of the design