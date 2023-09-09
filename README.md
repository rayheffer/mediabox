# MediaBox JavaScript Library
##Overview
MediaBox is a minimalist yet potent JavaScript library that elevates media display experience. It's perfect for developers who need a light yet powerful media display tool. It supports a wide array of media types including images, videos, and iframes.

## 🚀 Quick Start

### Hosting JavaScript and CSS yourself
To integrate MediaBox into your project, download the `mediabox.js` file and include it at the bottom of your HTML file:

``` html
    <!-- MediaBox JS -->
    <script src="path/to/mediabox.min.js"></script>
```

Do the same for `mediabox.min.css`, downloading it and including it on your page:

``` html
    <!-- MediaBox CSS -->
    <link rel="stylesheet" href="mediabox.css" type="text/css">
```

### Using a CDN (recommended for most) for the JavaScript and CSS
Instead of downloading and hosting the JavaScript and CSS yourself, you can simply use the CDN (Content Delivery Network) links. CDNs provide a great way to speed up your web project and offer a better user experience. CDNs provide fast, distributed access to static resources by serving them from the nearest location to each user.

**Note**: However, as a cybersecurity professional I personally take caution here. The external nature of a CDN means that you're relying on another platform to serve your files. If this platform, or even your own repository, gets compromised, malicious code could be distributed. This is true of any JavaScript library, not just this one. 

## 🏗️ HTML
Create an HTML element, apply the `.mediabox-link` class, and include a `data-src` attribute pointing to your desired media:

``` html
<div class="mediabox-link" data-src="image.jpg">
  <img src="thumbnail.jpg">
</div>
```

Feel free to use the included demo page (index.html) for quick tests.

## 🎬 Adding a Play Button
To overlay a play button, use the play-button-wrapper container. Add it after the image, as shown:

```html
<div class="mediabox-link" data-width="1000" data-url="https://www.youtube.com/embed/wTblbYqQQag?autoplay=1">
  <img src="jim.jpg" alt="Your Video Image" />
  <div class="play-button-wrapper">
    <div class="play-button"></div>
  </div>
</div>
```

## 🤔 Why Choose Between `mediabox.js` and `mediabox.min.js`?

### `mediabox.js`
Ideal for development purposes, the uncompressed version is your go-to if you wish to debug, extend functionalities, or dive into the nitty-gritty of the code.

### `mediabox.min.js`
For production, I recommend the minified version. It's stripped off any superfluous spaces, line breaks, and comments, resulting in a considerably lighter file primed for performance.

## 🎨 Custom Styling
For custom styles, your options are twofold:

1. Tweak the mediabox.css file directly.
2. Create your own stylesheet and go wild.

**Note**: The inline <style> section in index.html serves as a demo styling guide and isn't required for MediaBox's core functionality.