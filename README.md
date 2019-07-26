# Image Navigation Carousel

The image navigation carousel is a responsive, lightweight implementation of a carousel with image navigation.
Usually, other carousels use thumbnails as their image navigation, but what if you wanted to use logos?
I designed this carousel to make a replacement to the usual arrow, dot (bullet), or thumbnail carousel.

## Installation

To install, include the JavaScript and CSS.

## Usage

Just follow the following layout for the HTML implementation

```html
<!-- Slider container -->
<div class="slider">
    <ul class="slider-bullets">
        <!-- Left navigation button -->
        <button class="slider-navigation slider-navigation_left"><img src="/img/left-arrow.svg"/></button>
        <!-- Pair each bullet image with the corresponsing slide -->
        <li class="bullet"></li>
        <!-- Right navigation button -->
        <button class="slider-navigation slider-navigation_right"><img src="/img/right-arrow.svg"/></button>
    </ul>
    <!-- Slider gallery -->
    <ul class="slider-gallery">
        <!-- Each individual slide -->
        <li class="slide">
            <!-- Fill custom content here -->
        </li>
    </ul>
</div>
```  

## Custom CSS

Make sure you include your custom styles after the declaration from the default stylesheet
