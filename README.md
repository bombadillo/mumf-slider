# Mumf Slider

A basic jQuery plugin for generating sliders for HTML content and/or image galleries.

## Main Features

- Can be used for image galleries and HTML content.
- Fully responsive. Both on browser resize and between slides if difference in slide height exists.
- Easy to customize
   - The plugin is modular in that it's functions can be overwritten and added to. For instance you can add your own slide transition effect.
   - Custom themes can be created and used by adding them to the ```mumf-slider/themes/``` directory and adding a reference to it's CSS file.
   - Options can be changed on slider instantiation to enable/disable auto rotation, navigation, default thumbnails, and many more.



## Project Setup

What you'll need to get the project running

1. >= jQuery v1.9.0 for browsers other than IE < 10 which require >= jQuery v1.10.1 


## Deploying

Simply add a reference to the ```mumf-slider/js/mumf-slider.js``` file within your index.html, using a JavaScript require framework such as Head.js or however you include your JavaScript files.

## Markup Required before Slider Instantiation

### Basic Structure of slider

The basic structure of the slider is as follows:

```html
<!-- Slider container (The element you will use when instantiating slider) -->
<div class="slider">

    <!-- Used to hold all slides. -->
    <ul>
    
        <!-- Single slide. -->
        <li class="slide">
            <!-- This element level can either be a div or link element -->
            <div>           
                <!-- This level contains the slide content which can be simply images, 
                     HTML elements or a mix of the two.
                -->
                <img src="img/1.jpg" alt="1">
            </div>
        </li>
                       
    </ul>
</div>
```

### Basic Structure of thumbnails

If you want thumbnails to be used for navigation you can add the element within your slider element.

The basic structure of the slider thumbnails is as follows:

```html
<!-- Thumbnail container -->
<div class="thumbnails">
    <!-- Used to hold each thumbnail -->
    <ul>
        <!-- Single thumbnail -->
        <li class="">
            <!-- Container for thumbnail -->
            <div>                       
                <!-- You can use HTML or a simple image element -->
                <img src="img/1.jpg" alt="1">
            </div>
        </li>
    </ul>                    
</div>
```

### Image Slider

The HTML markup to be used for image sliders must use the following structure:  
```html
<div class="slider">
    <ul>
        <li class="slide">
            <!-- This element level can either be a div or link element -->
            <div>                                
                <img src="img/1.jpg" alt="1">
            </div>
        </li>
        <li class="slide">
            <!-- This element level can either be a div or link element -->
            <a href="http://link/to/content">
                <img src="img/2.jpg" alt="2">
            </a>
        </li>
        <li class="slide">
            <!-- This element level can either be a div or link element -->
            <div>
                <img src="img/3.jpg" alt="3">
            </div>
        </li>
        <li class="slide">
            <!-- This element level can either be a div or link element -->
            <div>
                <img src="img/4.jpg" alt="4">
            </div>
        </li>                        
    </ul>
</div>
```

### HTML Slider

The HTML markup to be used for image sliders must use the following structure:  
```html
<div class="slider">
    <ul>
        <li class="slide">
            <div>                                
                <!-- Your HTML content here. -->             
            </div>
        </li>    
        <li class="slide">
            <div>                                
                <div class="item">
                    <h4>Heading</h4>
                    <p>Paragraph</p>
                </div>
                <div class="item">
                    <h4>Heading</h4>
                    <p>Paragraph</p>
                </div>                
            </div>
        </li>
        <li class="slide">
            <div>                                
                <div class="item">
                    <h4>Heading</h4>
                    <p>Paragraph</p>
                </div>
                <div class="item">
                    <h4>Heading</h4>
                    <p>Paragraph</p>
                </div>                
            </div>
        </li>
    </ul>
</div>
```

### Slider with thumbnails

The HTML markup to be used for image sliders with thumbnail navigation must use the following structure:  

```html
<!-- Slider -->
<div class="slider">
    <ul>
        <li class="slide">
            <!-- This element level can either be a div or link element -->
            <div>                                
                <img src="img/1.jpg" alt="1">
            </div>
        </li>
        <li class="slide">
            <!-- This element level can either be a div or link element -->
            <a href="http://link/to/content">
                <img src="img/2.jpg" alt="2">
            </a>
        </li>
        <li class="slide">
            <!-- This element level can either be a div or link element -->
            <div>
                <img src="img/3.jpg" alt="3">
            </div>
        </li>
        <li class="slide">
            <!-- This element level can either be a div or link element -->
            <div>
                <img src="img/4.jpg" alt="4">
            </div>
        </li>                        
    </ul>

    <div class="thumbnails">
        <ul>
            <li class="">
                <div>                                
                    <img src="img/1.jpg" alt="1">
                </div>
            </li>
            <li class="">
                <div>
                    <img src="img/2.jpg" alt="2">
                </div>
            </li>
            <li class="">
                <div>
                    <img src="img/3.jpg" alt="3">
                </div>
            </li>
            <li class="">
                <div>
                    <img src="img/4.jpg" alt="4">
                </div>
            </li>                        
        </ul>                    
    </div>
</div>

    </div>
</div>
<!--/Slider -->
```

## Slider Types

- Basic slider instantiated using ```javascript $('.slider-fade').mumfSlider();``` will create a slider


