# scss-util

A bare bones SCSS utility framework that can be used as a starting point for simple site builds. To be used along with a reset such as [Normalize.css](https://necolas.github.io/normalize.css)

## Usage

Use the pre-complied css in the build directory or alternatively include the `src/styles.scss` into the SCSS complie process for the given project (gulp, webpack, scss cli etc).

## Customisation

Sizes, colors and breakpoints can be configured in `src/_variables.scss`

```scss
$font-family: 'Quicksand', sans-serif;
$base-font-size: 62.5%;

// General sizes, margins, padding, borders etc
$sizes: (
    0: 0px,
    1: 1px,
    4: 4px,
    5: 5px,
    10: 10px,
    15: 15px,
    20: 20px,
    25: 25px,
    30: 30px,
    35: 35px,
    40: 40px,
    150: 150px,
    180: 180px,
    300: 300px,
);
...
```

## Margin

| Property | Class |
|---|---|
| margin-top | .mt-{size} |
| margin-right | .mr-{size} |
| margin-bottom | .mb-{size} |
| margin-left | .ml-{size} |
| margin-left, margin-right | .mx-{size} |
| margin-top, margin-bottom | .my-{size} |
| margin | .m-{size} |
| margin: auto | .m-auto |

## Padding
| Property | Class |
|---|---|
| padding-top | .pt-{size}  |
| padding-right | .pr-{size}  |
| padding-bottom | .pb-{size}  |
| padding-left | .pl-{size}  |
| padding-left, padding-right | .px-{size} |
| padding-top, padding-bottom | .py-{size}  |
| padding | .p-{size}  |

## Width
| Property | Class |
|---|---|
| width | .w-{size} |
| width: 100vw | .vw-100 |
| width: 100% | .w-100perc |

## Height
| Property | Class |
|---|---|
| height | .h-{size} |
| height: 100vh | .vh-100 |
| width: 100% | .h-100perc |

## Flexbox

| Property | Class |
|---|---|
| display: flex | .flex |
| flex-direction: row | .flex-row |
| flex-direction: column | .flex-column |
| align-items: flex-start | .align-start |
| align-items: flex-end | .align-end |
| align-items: center | .align-center |
| justify-content: flex-start | .justify-start |
| justify-content: flex-end | .justify-end |
| justify-content: center | .justify-center |
| justify-content: space-around | .justify-around |
| justify-content: space-between | .justify-between |
| flex: 1 | .flex-1 |
| flex: 2 | .flex-2 |
| flex: 3 | .flex-3 |
| flex: 4 | .flex-4 |
| flex: 5 | .flex-5 |

## Colors
| Property | Class |
|---|---|
| background-color | .bg-{color} |
| color | .text-{color} |
| border-color | .border-{color} |

## Apperance
| Property | Class |
|---|---|
| cursor: pointer | .cursor-pointer |
| cursor: hand | .cursor-hand |
| text-decoration: none | .decoration-none |
| display: none | .hide |
| display: block | .show, .block |
| display: inline | .show-inline |
| overflow: hidden | .overflow-hidden |
| overflow-x: scroll | .overflow-x |
| overflow-y: scroll | .overflow-y |
| white-space: nowrap | .nowrap |

## Responsive

Responsive breakpoints can be configured within `src/_variables`. 

```scss
// Responsive breakpoints
$breakpoints: (
    'sm': 600px,
    'md': 900px,
    'lg': 1024px
);
```

Then simply prefix a breakpoint to any of the the above classes like so:

`.sm:mx-5 .md:mx-10`

`.sm:text-blue .lg:text-red`

`.sm:flex-column .lg:flex-row`