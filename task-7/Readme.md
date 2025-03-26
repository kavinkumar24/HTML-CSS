# Pure CSS Carousel/Slider

## Created a frame and inside that four images scroll infinite linear 

## Html Elements used
-  `<div id="gallery_container">` - Defines the frame with border to contain slides
- `<input type="radio" name="slider" id="slide1" checked>` - Defines a radio button which helps at the time of manual changing
- `<div class="slider-container">` - Defines a container which hides the image slides
- `<div class="slider">` - Defines the Screen present inside the slider-container
- `<div class="slide">` - Defines a each slide with image
- `<div class="navigation">` - Defines a container for positioning the navigation dots
- `<label for="slide1"></label>` - Act as a navigation to represent the slides

## CSS Elements used
- `display:flex` - Defines the layout of the page (Horizontal or vertical)
- `box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);` - gives a light shadow for frame which add visual interest to elements.
- ` overflow: hidden;` - It plays a crucial role in the slider which hides the image and return back to the container
``` 
@keyframes autoSlide {
    0% {
        transform: translateX(0%);
    }

    25% {
        transform: translateX(-100%);
    }

    50% {
        transform: translateX(-200%);
    }

    75% {
        transform: translateX(-300%);
    }

    100% {
        transform: translateX(0%);
    }
}
```
- This `@keyframes` animation helps to move the image in a X axis for auto sliding, at each interval of time it will moved and come back to its original position

```
.slider {
    display: flex;
    width: 400%;
    animation: autoSlide 4s infinite linear;
}
```
- This allows the autoSlide animation in a linear infinite manner which will moves the image with no Acceleration or Deceleration 

```
input[type="radio"] {
    display: none;
}
```
- Hides the radio button and make a click able opject with a id connectivity

```
#slide1:checked~.slider-container .slider {
    animation: none;
    transform: translateX(0%);
}

#slide2:checked~.slider-container .slider {
    animation: none;
    transform: translateX(-100%);
}

#slide3:checked~.slider-container .slider {
    animation: none;
    transform: translateX(-200%);
}

#slide4:checked~.slider-container .slider {
    animation: none;
    transform: translateX(-300%);
}
```
- This allow for manual scrolling, when manual scrolling activate the auto scrolling need to disable for user consistency
- `~` -  selects and apply all elements that are next siblings of a specified element.

## Output Images for Web View
![alt text](./assests/Output.gif)

## Output Images for Mobile View 
![alt text](./assests/image.png)