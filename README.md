# Lazy Loading Images with Slick-Slider
Having a prominent slider is often key to implementing a visually exceptional design. It must, however, be balanced with the need to maintain your site's performance. [Solodev](https://www.solodev.com/) shows how to lazy load images using built in [Slick Slider](http://kenwheeler.github.io/slick/) functions.

## Tutorial

For detailed instructions, view Solodev's [Lazy Loading Images using Slick Slider](https://www.solodev.com/blog/web-design/lazy-loading-images-using-slick-slider.stml) article.

## Demo

Check out a working example on [JSFiddle](https://jsfiddle.net/solodev/sobtocgc/).

## HTML

The form includes basic HTML markup:
```
<div class="ct-header ct-header--slider ct-slick-custom-dots" id="home">
  <div class="ct-slick-homepage" data-arrows="true" data-autoplay="true">
  
<div class="ct-header tablex item">
	<img data-lazy="images/slide1.jpg">
      <div class="ct-u-display-tablex">
        <div class="inner">
          <div class="container">
            <div class="row">
              <div class="col-md-8 col-lg-6 slider-inner">
                <h1 class="big">Big Data. Realtime Insight.</h1>
                <p>Leverage your data and improve marketing and sales ROI.</p>
                <a class="btn btn-transparent btn-lg text-uppercase" href="#">Learn More</a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="ct-header tablex item">
	<img data-lazy="images/slide2.jpg">
      <div class="ct-u-display-tablex">
        <div class="inner">
          <div class="container">
            <div class="row">
              <div class="col-md-8 col-lg-6 slider-inner">
                <h1 class="big">Disrupting Industries with Grace</h1>
                <p>WebCorpCo is at the forefront of digital marketing, content management, automated marketing, and more.</p>
                <a class="btn btn-transparent btn-lg text-uppercase" href="">Learn More</a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="ct-header tablex item"> 
	<img data-lazy="images/slide3.jpg">
      <div class="ct-u-display-tablex">
        <div class="inner">
          <div class="container">
            <div class="row">
              <div class="col-md-8 col-lg-6 slider-inner">
                <h1 class="big">Moving Business Forward</h1>
                <p>Learn how WebCorpCo can take your business to the next level.</p>
                <a class="btn btn-transparent btn-lg text-uppercase" href="">Learn More</a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    
  </div>
</div>
```

## CSS

All CSS is included in lazy-load-slick.css.

## JavaScript

In order to lazy load the images in the slider, you must call the Slick Slider specigic "lazyLoad" attribute:
```
<script type="text/javascript">
	$(document).ready(function(){
		$('.ct-slick-homepage').slick({
			lazyLoad: 'ondemand',
		});
	}); 
</script>
```

For a full list attributes you can use to customize your slider, visit [Slick Slider by Ken Wheeler](http://kenwheeler.github.io/slick/).

## External Includes

The form includes the following third-party resources:
```
<script type="text/javascript" src="https://code.jquery.com/jquery-1.11.1.min.js"></script>     
<script type="text/javascript" src="https://cdn.jsdelivr.net/jquery.slick/1.3.8/slick.min.js"></script>    
<script type="text/javascript" src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/js/bootstrap.min.js"></script>

<link rel="stylesheet" type="text/css" href="https://cdnjs.cloudflare.com/ajax/libs/slick-carousel/1.6.0/slick.min.css">  
<link rel="stylesheet" type="text/css" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/css/bootstrap.min.css">  
```