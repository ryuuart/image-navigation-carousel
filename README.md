# Image Navigation Carousel

The image navigation carousel is a responsive, lightweight implementation of a carousel with image navigation.
Usually, other carousels use thumbnails as their image navigation, but what if you wanted to use logos?
I designed this carousel to make a replacement to the usual arrow, dot (bullet), or thumbnail carousel.

## Installation

To install, include the JavaScript and CSS.

## Usage

Just follow the following layout for the HTML implementation. Make sure your bullet matches
the the respective slide. This is how they sync with each other. Wrong order would make the bullet
link to the wrong slide ☝️

```html
<!-- Slider container -->
<div class="slider">
    <ul class="slider-bullets">
        <!-- Left navigation button -->
        <button class="slider-navigation slider-navigation_left"><img src="/img/left-arrow.svg"/></button>
        <!-- Pair each bullet image with the corresponsing slide -->
        <li class="bullet">
            <!-- Insert bullet content here -->
        </li>
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

## Customization

To customize or extend, just add onto the Incarousel CSS.

### Details about CSS classes

`slider`  
The slider container class  

`slider-bullets`  
The bullet container class.  

`bullet`  
Styling for a bullet. A bullet is an individual navigation item in the carousel.  

`slider-navigation`  
The slider navigation container class  

`slider-navigation_left` `slider-navigation_right`  
Styles each slider navigation button individually  

`slider-gallery`  
Container for all slides.  

`slide`  
An individual "slide" of content.  

`bullet-hide`  
Makes the bullet `display: none` without actually using `display:none`  

`bullet-active`  
highlights the active bullet  

`slide-active`  
reveals the current syncrhonized slide  

### Structuring the CSS

Make sure to use CSS specificity as much as possible (this is so the CSS doesn't meld in with your CSS).
For my examples, I made a separate stylesheet and overwrote the styles.

#### Example

```css
.slider .slider-gallery {
    margin: 0;
    width: 100vw;
    max-width: 100vw;
}

.slider .slider-bullets .bullet {
    padding: 0 0.75rem;
}

.slider .slider-bullets .bullet img {
    width: 5rem;
}
.slider .slider-bullets .bullet.bullet-hide img {
    width: 0;
}
```
