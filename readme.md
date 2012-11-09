# jQuery TouchTouch

A jQuery 1.7 plugin that makes it easy to display a set of photos on your site as a touch-optimized photo gallery.

## Highlights

* Smooth CSS3 animations and transitions;
* A responsive CSS interface that fills the screen and responds to changes in device orientation;
* Preloads photos only when they are needed;
* Supports swiping through photos;
* Displays onscreen arrows and listens for arrow key presses on desktop browsers;

## How to use

Using it is simple. Drop the <strong>touchTouch</strong> folder (you can find it in the download under <em>assets/</em>) somewhere in your website folder tree. After this, include <strong>touchTouch/touchTouch.css</strong> in your &lt;head&gt;, and <strong>touchTouch.jquery.js</strong> right after the jQuery library. The script depends on <strong>jQuery 1.7</strong> or above.

After you do all this, simply call the gallery as a regular jQuery plugin:

```js
$(function(){

	// Initialize the gallery
	$('#thumbs a').touchTouch();

});
```

You must pass anchor elements which point to images in their href attributes for the gallery to work. In addition to conveying which images are to be displayed in the gallery, this also provides a graceful fallback in case JavaScript is not available.

### Multiple Galleries

To show specific sets of pictures, add a "data-gallery" attribute to the anchor tags you want in that set, with a unique value. If this attribute isn't added, all images will be displayed.

```html
	<a href="http://farm8.staticflickr.com/7013/6754656011_3de2cc73a2_z.jpg" data-gallery="hongkong" style="background-image:url(http://farm8.staticflickr.com/7013/6754656011_3de2cc73a2_m.jpg)" title="Lion Rock"></a>
```

## License

Released under the MIT license

## Demo

Go to [Tutorialzine](http://tutorialzine.com/2012/04/mobile-touch-gallery/) for a live demo.