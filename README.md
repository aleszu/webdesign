# Story and Code: A Front-end Web Design Bootcamp 
Northeastern University's Media Innovation program

### The skills we’ll be covering

*How to get started with a HTML/CSS framework (standalone interactives like [What Would It Take To Turn Red States Blue? from FiveThirtyEight](https://projects.fivethirtyeight.com/2016-swing-the-election/), [Undue Force from the Baltimore Sun](http://data.baltimoresun.com/news/police-settlements/) and [Spies in the Skies from BuzzFeed](https://www.buzzfeed.com/peteraldhous/spies-in-the-skies?utm_term=.hhenRxQPy1#.kgP31Xg2No) are built with custom code outside of the regular CMSs.) Knowing how to code that up is essential if you want to add interactivity to your story. 

*How to envision and code a small menu of CSS animations and jQuery elements. This is the fun stuff: transitions, scroll-based animations, reveals, hovers, etc. Ever wonder how [The Pudding](https://pudding.cool) works? We’ll get you started coding these little gizmos. 

*We all have different levels of experience with HTML, CSS and Javascript. The goal of this bootcamp is to get us all roughly on the same page.*

# Booting up a standalone webpage using Skeleton 

To layout an article, it helps to have a grid and a system to organize all your interconnected elements. In web design, this is called a framework. These frameworks are packages that structure your HTML, your CSS and other related elements like Javascript documents. Some frameworks you may have heard of: Bootstrap, Foundation, Groundwork, Gumby, and Skeleton. 

[Skeleton](http://getskeleton.com/), which is one of the most bare bones responsive frameworks out there, is what we'll be using for this workshop.

### Download Skeleton 

Download Skeleton, unzip it and open up the entire folder in a text editor like [Sublime Text 2](http://www.sublimetext.com/2). 

![img1](http://www.storybench.org/wp-content/uploads/2015/08/skeleton_html1-1440x760.png)

### Take a tour of the index page

Look for the `<html>, <head>, and <body>` tags.

### Add a title, description and author in the `<head>`

Take a look around and try to understand what all is being laid out in the `<head>` of your index.html page. Start by adding your title, description and author.

### Add a full-bleed hero image and then overlay text

Paste in the following just before the `<div class="container">` tag. Link to a large image (ideally over 2,000 pixels wide) in `src=`.

```
<div class="hero">
    <img src="http://aleszu.com/workshops/webdesign/images/hero.jpg" style="width:100%" />
  <div class="hero-text">
    <h1>Big Bold Headline</h1>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
  </div>  
</div>
```

To style the text, add this to the *skeleton.css*. It's good practice to include a full font stack in case the browser can't render your first choice.

```

.hero-text h1{
  color: #e0e0eb;
  font-family: Baskerville, "Baskerville Old Face", "Goudy Old Style", Garamond, "Times New Roman", serif;
  font-size: 4.1em;
  margin: auto;
  position: absolute; 
  text-align: center; 
  top: 360px;
  left: 0;
  right: 0;
  bottom: 0;
  z-index: 1;
}

.hero-text p{
  font-size: 1.5em;
  color: #e0e0eb;
  font-family: Baskerville, "Baskerville Old Face", "Goudy Old Style", Garamond, "Times New Roman", serif;
  margin: auto;
  position: absolute; 
  text-align: center; 
  top: 420px;
  left: 0;
  right: 0;
  bottom: 0;
  z-index: 1;
}

``` 

### Preview the page

Open the index.html from your Skeleton folder in a browser to preview the page you've been building.

![image](http://aleszu.com/workshops/webdesign/images/overlaytext.png)

### Add content to the `<body>`

Be sure to reference the Skeleton [documentation](http://getskeleton.com/) before adding text willy-nilly. Plan out, ideally by hand, how you want to layout your text, photos, pullquotes and interactive elements.

For now, let's add five paragraphs of placeholder text. Designers love to use pseudo-Latin as dummy text for mocking up layouts. (Origin story [here](http://www.straightdope.com/columns/read/2290/what-does-the-filler-text-lorem-ipsum-mean)).

Notice that we're adding paragraph tags to denote the beginning and end of the grafs: `<p>` and `</p>`. Also notice that we're nesting the text inside of a "column" which is inside a "row" which is inside a "container."

```
<div class="container">
<div class="row">
<div class="column" style="margin-top: 15%">

<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus sed maximus mi, sed ullamcorper ante. Vivamus tristique dui eget molestie molestie. Pellentesque ex tortor, eleifend volutpat lorem eu, commodo vulputate erat. Phasellus a nisi mauris. Sed fringilla, nisi sed varius elementum, enim ipsum luctus libero, commodo lacinia quam sem sed felis. Aenean lectus neque, malesuada non dolor a, ultrices pulvinar eros. Aenean id est at sapien lobortis interdum ac eu massa. Nam vulputate sollicitudin erat, a finibus velit fringilla id. Vestibulum massa lorem, finibus vel nunc sed, rhoncus consectetur est. Praesent non urna posuere, auctor ante at, blandit nibh. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse potenti. Aliquam consequat porta quam, sed vulputate est ornare eget.</p>

<p>Maecenas sed felis sit amet nibh efficitur tincidunt. Maecenas in metus facilisis, vulputate est a, volutpat ante. In hac habitasse platea dictumst. Donec quis venenatis tellus, ac varius neque. Suspendisse lacinia, elit vitae ullamcorper vestibulum, justo nisi auctor eros, sit amet elementum dui ex sit amet libero. Nullam fringilla scelerisque pellentesque. Curabitur sodales consequat nulla, sed auctor sem sollicitudin ac. Phasellus quis dui non leo aliquet posuere. Cras posuere sollicitudin magna in rutrum. Quisque eget mi ante. Nullam ullamcorper vitae sem et consectetur.</p>

<p>Pellentesque ullamcorper posuere ex nec malesuada. Cras neque ex, sollicitudin vitae eleifend sed, pellentesque eu sem. Vivamus egestas tincidunt mi. Vivamus id libero id lorem varius faucibus. Integer lacus ligula, aliquet imperdiet hendrerit vel, congue nec mauris. Maecenas eu maximus purus. Fusce id feugiat est, eget convallis lorem. Ut semper sapien aliquet tristique semper. Maecenas ornare lacinia leo, sit amet interdum augue sollicitudin vitae. Vestibulum malesuada purus at molestie maximus.</p>

<p>Phasellus non faucibus turpis, vitae placerat erat. Donec vestibulum dapibus lacus a rutrum. Etiam eget elementum justo. Sed nec est eu lectus placerat consectetur. Fusce a dapibus quam, vitae facilisis mauris. Donec volutpat sit amet sapien a rutrum. Morbi vitae aliquam nisl. Morbi suscipit congue velit ac laoreet. Phasellus egestas ipsum tortor, in laoreet urna dictum et. Suspendisse eget purus at ante sollicitudin varius. Pellentesque iaculis efficitur fermentum. Pellentesque porta faucibus tellus sed facilisis. Nunc dignissim neque in nibh porttitor eleifend. Proin id tortor eleifend, aliquam diam rutrum, convallis metus. Curabitur sed facilisis dui. Morbi nulla quam, rhoncus sed tempor non, lobortis posuere nulla.</p>

<p>Nam vestibulum eu sem eget tempor. Nunc volutpat convallis ullamcorper. Sed lobortis elementum sollicitudin. Vivamus vestibulum pulvinar velit eu volutpat. Sed id dictum sem. Nam mollis suscipit mauris, laoreet interdum odio laoreet in. In accumsan auctor ante. Etiam consectetur, lacus at maximus convallis, libero sem tincidunt est, at viverra turpis dolor a diam. Maecenas eros nisi, aliquet sed felis eget, faucibus feugiat libero. Pellentesque consectetur, sapien vel facilisis posuere, leo diam rhoncus leo, eget pellentesque turpis nunc ut nisl.</p>

</div>
</div>
</div>
``` 

### Change the body font

Go to [Google Fonts](https://fonts.google.com/) and look for a new font. I've chosen [Open Sans](https://fonts.google.com/specimen/Open+Sans?selection.family=Open+Sans), a sans-serif font that's extremely popular online. To add it to your page, you need to change the URL where you're calling the font in the `<head>`.  

```
  <!-- FONT
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <link href="https://fonts.googleapis.com/css?family=Open+Sans" rel="stylesheet">
```

You also need to open the **skeleton.css** file and change the CSS.

### Inspect the CSS and design a dropcap

Open skeleton.css and go to line 127. Change Raleway to Open Sans: 

```
font-family: "Open Sans", "HelveticaNeue", "Helvetica Neue", Helvetica, Arial, sans-serif;
```

Let's add some CSS to design a dropcap plus a subtitle for our custom CSS:

```
/* Custom CSS
–––––––––––––––––––––––––––––––––––––––––––––––––– */

.dropcap {
  font-size: 2.8em;
  float: left;
  line-height: 1;
  margin-right: 9px;
  margin-top: 5px;
}
``` 

Now, if you add the "dropcap" class to a `<span>` element, you can apply this styling to a single letter. Let's do that for the first letter of the first paragraph:

```
<p><span class="dropcap">L</span>orem ipsum dolor sit amet...
```

![dropcap](http://aleszu.com/workshops/webdesign/images/dropcap.png)

# Coding a couple of gizmos using CSS, jQuery and D3plus

### Adding a basic animation

As a proof of concept, let's add a left-floated image that is replaced with another image when the user hovers a mouse over it. Using `onmouseover` and `onmouseout` in the `<img>` tag, we point to the two images. 

```
<div class="u-pull-left">
    <img class="img-left" src="http://aleszu.com/workshops/webdesign/images/calame.jpg" onmouseover="this.src='http://aleszu.com/workshops/webdesign/images/calame2.jpg'" onmouseout="this.src='http://aleszu.com/workshops/webdesign/images/calame.jpg'" />
</div>
```

The `u-pull-left` class is from Skeleton and will float the image to the left. The `img-left` class is a custom one we've added. Let's customize the size of the image using that class. Add this to your **skeleton.css** file. 

```
.img-left{
  width: 400px;
  padding: 10px 50px 0px 30px;
}
```  

Refresh the page and see your simple animation take effect. 

### Adding a jQuery element

Let's add a typewriter-style animation using jQuery. First, add the following subtitle (using the `<h2>` header tags) above the first paragraph. Notice the subtitle “Nit-picking and navel-gazing” has two classes assigned to it.

```
<h2 class="revealScrollhidden scrollReveal">“Nit-picking and navel-gazing”</h2>
```

#### Write the custom script

Now, open up a new file in your text editor. Paste the following script in and save it as **scroll.js**, storing it in a new folder called "js" withing your main Skeleton directory.

```
$(window).scroll(function () {
    $('.scrollReveal').each(function () {
        var imagePos = $(this).offset().top - 310;
        var imageHeight = $(this).height();
        var topOfWindow = $(window).scrollTop();
        if (imagePos < topOfWindow + imageHeight && imagePos + imageHeight > topOfWindow) {
            $(this).addClass("typewriter");
        } 
    });
});
```

What is this script doing? It applies the typewriter class to any element already containing the "scrollReveal" class, which in our case is a subtitle `<h2>`. The script also only executes the function if the user has scrolled to a specific position, which is a distant from the top of the viewing window. In other words, the script will only trigger once that position has been reached. (This also ensures all subsequent subtitles will only be triggered once they are reached, as opposed to all being triggered once the page is loaded.) 

#### Call the jQuery

Next, call the jQuery in the `<head>`. We'll need that to run the jQuery we're about to include. 

```
<!-- Scripts
–––––––––––––––––––––––––––––––––––––––––––––––––– -->
<script src="http://ajax.googleapis.com/ajax/libs/jquery/2.1.1/jquery.min.js"></script> 
```

#### Call the script

Call that **scroll.js** script in the `<head>` of your index.html.

```
<!-- Scripts
–––––––––––––––––––––––––––––––––––––––––––––––––– -->
<script src="http://ajax.googleapis.com/ajax/libs/jquery/2.1.1/jquery.min.js"></script> 
<script src="js/scroll.js"></script>
```

#### Add the CSS

In **skeleton.css** add the following CSS:

```
/* Typewriter effect */

.revealScrollhidden {
   visibility: hidden;
}

.typewriter {
  visibility: visible;
  overflow: hidden; /* Ensures the content is not revealed until the animation */
  border-right: .15em solid black; /* The typwriter cursor */
  white-space: nowrap; /* Keeps the content on a single line */
  margin: 0 auto; /* Gives that scrolling effect as the typing happens */
  letter-spacing: .15em; /* Adjust as needed */
  margin-bottom: 2rem;
  font-family: Baskerville, 'Baskerville Old Face', 'Hoefler Text', Garamond, 'Times New Roman', serif;
  font-size: 4.0rem; 
  font-weight: bold;
  animation: 
    typing 3.5s steps(40, end),
    blink-caret .75s step-end infinite;
}

@keyframes typing {
  from { width: 0 }
  to { width: 100% }
}

@keyframes blink-caret {
  from, to { border-color: transparent }
  50% { border-color: black; }
}
```

Refresh the page and check out the subtitle at work. Add a few more "Lorem ipsum" grafs and precede them with a subtitle. As long as it has the `revealScrollhidden scrollReveal` classes, it will animate.  

### Adding an interactive chart

[Highcharts.js](https://www.highcharts.com) is becoming a popular [alternative](http://www.storybench.org/seattles-kcts9-building-digital-first-newsroom-culture/) to [D3js](d3js.org) in [newsrooms](https://www.pri.org/stories/2017-07-14/more-75-percent-terrorist-attacks-2016-took-place-just-10-countries) around the country, though it requires a license and therefore is not free. 

We'll insert a highcharts [demo](https://www.highcharts.com/demo/line-time-series) whose text I've messed around with.  

#### Call the highcharts libraries

Call these two highcharts libraries in the `<head>` of index.html.

```
<!-- Scripts
–––––––––––––––––––––––––––––––––––––––––––––––––– -->
<script src="https://code.jquery.com/jquery-3.1.1.min.js"></script>
<script src="http://aleszu.com/workshops/webdesign/js/scroll.js"></script>
<script src="https://code.highcharts.com/highcharts.js"></script>
<script src="https://code.highcharts.com/modules/exporting.js"></script>
```

#### Insert the `<div>` that will hold the chart

Add some more paragraphs of dummy text and insert the following `<div>`. Notice that we're defining some dimensions and adding a 50px bottom-margin. So the text isn't scrunched up against the chart.

```
<div id="container" style="min-width: 310px; height: 400px; margin: 0 0 50px 0"></div>
```

#### Add the javascript

Directly into the close `</body>` tag, add this script:

```
<script type="text/javascript">

$.getJSON('https://www.highcharts.com/samples/data/jsonp.php?filename=usdeur.json&callback=?', function (data) {

    Highcharts.chart('container', {
        chart: {
            zoomType: 'x'
        },
        title: {
            text: 'New York Times digital subscribers'
        },
        subtitle: {
       //     text: document.ontouchstart === undefined ?
       //             'Click and drag in the plot area to zoom in' : 'Pinch the chart to zoom in'
        },
        xAxis: {
            type: 'datetime'
        },
        yAxis: {
            title: {
                text: 'Million subscribers'
            }
        },
        legend: {
            enabled: false
        },
        plotOptions: {
            area: {
                fillColor: {
                    linearGradient: {
                        x1: 0,
                        y1: 0,
                        x2: 0,
                        y2: 1
                    },
                    stops: [
                        [0, Highcharts.getOptions().colors[0]],
                        [1, Highcharts.Color(Highcharts.getOptions().colors[0]).setOpacity(0).get('rgba')]
                    ]
                },
                marker: {
                    radius: 2
                },
                lineWidth: 1,
                states: {
                    hover: {
                        lineWidth: 1
                    }
                },
                threshold: null
            }
        },

        series: [{
            type: 'area',
            name: 'Subscribers',
            data: data
        }]
    });
});

</script>
```

Refresh the page. Voila! 




