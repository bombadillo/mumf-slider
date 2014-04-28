# Mumf Slider

A basic jQuery plugin for generating sliders for HTML content and/or image galleries.

## Project Setup

What you'll need to get the project running

1. >= jQuery 1.9.0


## Deploying

Simply add a reference to the ```mumf-slider/js/mumf-slider.js``` file within your index.html, using a JavaScript require framework such as Head.js or however you include your JavaScript files.

## Markup Required before Slider Instantiation

The HTML markup to be used for sliders must use the following structure:  
```html
                <div class="slider-slide">
                    <ul>
                        <li class="slide">
                            <div>                                
                                <img src="img/1.jpg" alt="1">
                            </div>
                        </li>
                        <li class="slide">
                            <div>
                                <img src="img/2.jpg" alt="2">
                            </div>
                        </li>
                        <li class="slide">
                            <div>
                                <img src="img/3.jpg" alt="3">
                            </div>
                        </li>
                        <li class="slide">
                            <div>
                                <img src="img/4.jpg" alt="4">
                            </div>
                        </li>                        
                    </ul>
                </div>
```

## Slider Types

- Basic slider instantiated using ```$('.slider-fade').mumfSlider();``` will create a slider


