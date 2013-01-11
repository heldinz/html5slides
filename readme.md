# HTML5 Slide Template

## Using the template

* Download the template project using the 'Download' button from GitHub.
* Create a directory for your presentation
* Unzip the template files in _DIR/template_
* Create _DIR/slides.html_ (you can change the name of course)
* In the HMTL slides, load the following script:
    ```<script src='template/slides.js'></script>```
	
* Create the _section_ containing your slides:
	```<section class='slides layout-regular template-arrow-ubidreams'></section>```
		
* Each ```<article>``` created within this section is a slide

## Changing the _template_ path

If you want to customized the location of the template, you need to update the _TEMPLATE\_PATH_ variable before loading the script:

	<!-- Customize TEMPLATE_PATH -->
	<script>
		var TEMPLATE_PATH="../";
	</script>
    <script src='../slides.js'></script>

By default _TEMPLATE\_PATH is set to _template/_

## Updating the style

The style is developed with [Less](http://lesscss.org/).

1. Update the _styles.less_ file.
2. Recompile the the less file with:

	lessc styles.less > styles.css
	
