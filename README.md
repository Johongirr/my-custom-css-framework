# Custom CSS Framework

> ### Project part of Odin [curriculum](https://www.theodinproject.com/lessons/design-your-own-grid-based-framework)
> ### Visit to [view](https://johongirr.github.io/my-custom-css-framework/) a project

## Built with
 * HTML5
 * CSS3 (GRID,FLEXBOX,RWD)
 * SASS



## Overview
This is 12-column responsive CSS grid famework built with Flexbox with mobile-first approach


## How It Works

### Breakpoints
In this framework there are 5 breakpoints and I used min-width in media queries as this framework' focusses on the **mobile-first** approach and progressively change the layout to fit larger screens. These breakpoints are as followings
* 576px = sm
* 768px = md
* 992px = lg
* 1200px = xl
* 1400px = xxl 

### Grid Container 
There are 3 types of containers with the class of as followings.
* **container-fluid** - stays 100% wide in all breakpoints
* **container** - is fixed container that starts 100% wide in **xs** screens and then in each breakpoint its max-width is set to new value
* **container-{breakpoint}** - that stays 100% wide until breakpoint and in each breakpoin its max-width is changed to new value
For example: you can create container with break point like this
```HTML
    <div class="container-md">
        <div class="row">
            Cols
        </div>
    </div>
```


### Row
I made a class of row to be a flex container and it needs to be nested inside container class. As it's flexbox container, you can use all flex container properties that I predefined for you. 
Example:
```HTML
    <div class="container-md">
        <div class="row justify-content-between align-items-center">
            Cols
        </div>
    </div>

```


### Columns
You can create columns on each breakpoint by specifying how many column each column occupies. 
Example: 
    * In this example we created 4 columns and amount of columns they occupy changes in each breakpoint
        * When viewport size is extra small all of them occupy all 12 columns
        * And then when small breakpoint hits, they each occup 6 columns
        * On medium screens they occupy 3 of 12 columns
        * And lastly when the screen is large they all occupy 4 of 12 columns
```HTML
    <div class="container">
        <div class="row">
            <div class="col-12 col-sm-6 col-md-3 col-lg-4">
                Content
            </div>
            <div class="col-12 col-sm-6 col-md-3 col-lg-4">
                Content
            </div>
            <div class="col-12 col-sm-6 col-md-3 col-lg-4">
                Content
            </div>
            <div class="col-12 col-sm-6 col-md-3 col-lg-4">
                Content
            </div>
        </div>
    </div>

```


### Gutters
I created gutter for both vertical and horizontal spacing in between columns. You can set gutters in any breakpoint as you wish.

Example: As you can in this example, I'm changing gutter in between both rows and columns in each breakpoint
```HTML
    <div class="container">
        <div class="row g-1 g-sm-2 g-md-3 g-lg-4 g-xl-5">
            <div class="col-12 col-sm-6 col-md-3 col-lg-4">
                Content
            </div>
            <div class="col-12 col-sm-6 col-md-3 col-lg-4">
                Content
            </div>
            <div class="col-12 col-sm-6 col-md-3 col-lg-4">
                Content
            </div>
            <div class="col-12 col-sm-6 col-md-3 col-lg-4">
                Content
            </div>
        </div>
    </div>
```


## Author
:man: Johongir 
* Github [Johongir](https://github.com/Johongirr)

## Show your support
Give a :star: if u like this project


## Contributing
Contributions, [issues]() and feature requests are welcome!


## Licence
The project is licenced under the MIT licence
