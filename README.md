# jQuery plugin: Easy Accordion

[https://www.madeincima.it](https://www.madeincima.it "https://www.madeincima.it")

## How does it work?
Easy Accordion plugin will get your **definition lists** (DTs) and generate a nice and smooth horizontal accordion. You can then decide to make it a timed slideshow or leave it still.
As usual, all of that will be realized in an unobtrusive, SEO friendly and accessible way.

## Features
* Easily create a **nice and smooth accordion** effect
* Decide whether or not automatically **animate your slider**
* Insert **multiple instances** of the accordion in the same page
* Set the **active slide** when the user loads the page
* Include or remove the **slide number**
* **Text is rotated using CSS** properties. No need for images!
* Easy Accordion is **totally customizable** via CSS: change height, width, set borders and paddings, use background images and so on
* **Accessible** and **SEO friendly**
* **Slide any kind of content** (divs, simple text, images, lists, etc.)
* **Less than 8KB!**
* **No dependencies** at all!

## Usage
Here is the HTML code for a simple definition list wrapped into a div container:

Title slide
You can put here any kind of content (divs, text, images, etc.)…
One more
You can put here any kind of content (divs, text, images, etc.)…
Another slide
You can put here any kind of content (divs, text, images, etc.)…
We need now to include three different files in the head of the document: the jQuery library, the Easy Accordion plugin and our Script file from where we’re going to call the plugin. If you do not know yet how to set up your jQuery environment, you can find a detailed explanation in my first jQuery tutorial, otherwise just keep reading!

You can target any definition list using the powerful JQuery-selectors. The plugin accepts different arguments.

## Parameters
Make sure you wrap your definition list into a div container and call the plugin on the div element and not on the definition list straight away:
```javascript
$('#your-accordion-container').easyAccordion();
```
If you don’t pass any parameter to the plugin it will generate a simple accordion with slide numbers and no autoplay by default. To see the hidden slides userswill have to click on the respective slide titles.

To enable the autoplay you simply have to set the “autoStart” parameter to “true” and the “slideInterval” ( in milliseconds) to a number as follow:
```javascript
$('#your-accordion-container').easyAccordion({
   autoStart: true,
   slideInterval: 5000
});
```
In this example the plugin will move to the next slide every 5 seconds. As soon as it gets to the last slide it starts over again. If you click on one of the slides the slideshow stops so that the user can easily read the content or move back and forth.

You can also remove the slide numbers by setting the “slideNum” parameter to “false” as follow:
```javascript
$('#your-accordion-container').easyAccordion({
   autoStart: true,
   slideInterval: 3000,
   slideNum: false
});
```

## Browser support
The jQuery Easy Accordion plugin has been tested on the following browsers:
Firefox 3.5+, IE6/7/8, Safari 5+ and Google Chrome.

