## Welcome ##

FanGate is an open source Facebook Page tab framework with built-in support for showing different content to fans and non-fans. It should require minimal knowledge of PHP and allow anyone who knows HTML to upload a gated fan page tab.

## How to use it ##

### Requirements ###

 * A PHP-enabled server with the cURL and JSON enabled.
 * A Facebook account
 * A Facebook Page (not your profile)

### Create the Facebook app ###

 1. To get started, head over to the [Facebook Developer App][1] to create an app of your own. Name it whatever you want, give it a namespace (whatever you want) and enter the human verification test to proceed to the settings page.

 2. This is about how the app settings should look:
   
 ![Settings screenshot](https://raw.github.com/jimmysawczuk/fangate/master/images/dev-settings.png)

### Create your tab ###

 1. [Download the framework from here][2] and extract it to your hard drive (you can also clone it from whatever code hosting site you're viewing this from).
 
 2. Open the `tpl` folder, and edit `like.html` and `nolike.html` to whatever you want. These are the files that are shown to fans and non-fans respectively. Edit them as you want. You can make style changes in `css/style.css` as that CSS file is included by default. Add images to whatever directory you want and reference them relatively or absolutely, keeping in mind that although the HTML files are in `tpl/`, they'll be served from the root of the FanGate framework.

Once you've made all the changes you want, upload them to your server and ensure they're at the same path you set in your App configuration.

### Install the app to your page ###
 1. Open `set-up.php` on your server (`http://yourdomain.com/path/to/tab/set-up.php`). Input your App ID and App Secret, and copy the results as instructed into a file called `config.php` in the same directory as `set-up.php`.
 
 2. Click "Install" and install the app to the page you want.
 
 3. (Optional) Delete or rename `set-up.php`.

## License

    The MIT License (MIT)
    Copyright (C) 2011-2012 by Jimmy Sawczuk

    Permission is hereby granted, free of charge, to any person obtaining a copy
    of this software and associated documentation files (the "Software"), to deal
    in the Software without restriction, including without limitation the rights
    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
    copies of the Software, and to permit persons to whom the Software is
    furnished to do so, subject to the following conditions:

    The above copyright notice and this permission notice shall be included in
    all copies or substantial portions of the Software.

    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
    THE SOFTWARE.

  [1]: http://www.facebook.com/developers
  [2]: https://github.com/jimmysawczuk/fangate/zipball/master