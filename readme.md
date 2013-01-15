# HTML5 Slide Template

## Using the template

* Download the template project using the 'ZIP' button from GitHub.
* Unzip the files
* Edit _index.html_ (you can change the name of course) to add your slides
* Each ```<article>``` created within the following section is a slide:
	```<section class='slides layout-regular template-akquinet'></section>```
* The ```template-akquinet``` class controls which logo appears on each slide.

## Changing the _template_ path

If you want to customize the location of the template, you need to update the _TEMPLATE\_PATH_ variable before loading the script:

	<!-- Customize TEMPLATE_PATH, default is to offline -->
    <script>
      //var PERMANENT_URL_PREFIX = 'http://html5-slides-template.googlecode.com/git/';
      //var TEMPLATE_PATH=PERMANENT_URL_PREFIX + "template/";
    </script>

By default, _TEMPLATE\_PATH is set to _template/_. You can change it to whatever you want, but we've provided a URL at which you
can find the default styles.

If you want to keep everything online (so that you can distribute one single HTML file, if you have linked all your
slide images from, say, Dropbox for example), you can change the location of _slides.js_ too.

    <!-- Default to using offline resources -->
    <script src='slides.js'>&#160;</script>
    <!-- Alternatively, load everything remotely, even slides.js -->
    <!--script src='http://html5-slides-template.googlecode.com/git/slides.js'>&#160;</script-->


## Updating the style

The style is developed with [LESS](http://lesscss.org/).

1. Update the _styles.less_ file.
2. Recompile the the less file with:

	lessc styles.less styles.css
	
## Adding themes

* Add logos to _templates/images_.
* Add styles to _styles.less_ and recompile.
* Replace the ```template-akquinet``` class in your HTML file with your new theme name.
