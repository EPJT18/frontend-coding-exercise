# [Swoop Aero](https://www.swoop.aero) - Coding Exercise (Frontend)
[![license][license-image]][license-link]

[license-image]: https://img.shields.io/badge/license-MIT-green
[license-link]: https://github.com/EPJT18/frontend-coding-exercise/blob/main/LICENSE

This coding exercise is used to challenge candidates applying to work for [Swoop Aero](https://www.swoop.aero)

## Instructions

* Create a React application that shows a Map.
* The Map should display features that mark the different localities in Victoria, Australia (plus parts of SA, ACT and NSW). Use the geojson data in the [Assets](#assets) section.
* Each feature or marker is clickable and should display the information about it. It will be up to you how to display this.
* The information about each marker can be read from the "properties" attribute of the Feature object.
```
# example

{
    "type": "Feature",
    "id": "VMFEAT_LOCALITY_POINT.60252",
    "geometry":
    {
        "type": "Point",
        "coordinates":
        [
            143.481649,
            -35.237661
        ]
    },
    "geometry_name": "SHAPE",
    "properties":
    {
        "PFI": 1582,
        "NAME_ID": 100374,
        "PLACE_NAME": "BEVERFORD",
        "PLACE_NAME_LABEL": "Beverford",
        "FEATURE_TYPE_CODE": "place",
        "FEATURE_SUBTYPE": "locality bounded",
        "HIERARCHY": 8,
        "STATE": "VIC",
        "SCALE_USE_CODE": "6",
        "PFI_CREATED": "2009-12-31Z",
        "UFI_CREATED": "2011-08-11Z",
        "OBJECTID": 582
    }
}
```
* Make sure to create git commits to give us an idea how you did all the work.
* And lastly, don't forget to write tests too.

## Layout
* Header (add a logo)
* Body/Map
* Footer (add some copyright text)

<em>See sample layout and info display [below](#sample-designs)</em>.

## Output / Expectations
* Provide us with a Github repo of your code. You can set it to private if you want and give us access so we can clone.
* Once we've cloned your repo, these are the only commands that we will execute
    * yarn install
    * yarn test
    * yarn start
* We will review your repository structure, code, app design and it's responsiveness.
* Ultimately, impress us with your UI skills! The general layout is simple. It's up to you to add more value to what you're coding.

## Technologies/Libraries

* React
* State management (any):
    * Redux Toolkit (preferred)
    * Mobx
    * React Context
* Map lib (any)
    * Openlayers (preferred)
    * Leaflet
* Test (any)
    * Jest
    * Mocha
    * Chai
    * Jasmine
    * Enzyme
    * Cypress IO
    * React-testing-library
    * Puppeteer
* User Interface (any)
    * MUI (preferred)
    * Bootstrap
    * AntD
    * Semantic UI

## Assets
* [swoop-logo.svg](/image/swoop-logo.svg) - logo
* [localities.json](/asset/localities.json) - (data sourced from [https://services.land.vic.gov.au/](https://services.land.vic.gov.au/))

## Sample Designs

* Clicking on a feature opens a bubble popup that displays the information about it.

    ![](/image/design-bubble.png)

* Clicking on a feature opens a dialog or modal that displays the information about it.

    ![](/image/design-bottom-right.png)

* Clicking on a feature opens a section at the bottom (just above the footer) that displays the information about it.

    ![](/image/design-bottom.png)

---
<h6 align="center">
    © 2022 <a href="https://www.swoop.aero" target="_blank">Swoop Aero</a>
</h6>