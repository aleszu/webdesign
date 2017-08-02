# Story and Code: A Front-end Web Design Bootcamp 
Northeastern University's Media Innovation program

### The skills we’ll be covering

⋅⋅*How to get started with a HTML/CSS framework (standalone interactives like [What Would It Take To Turn Red States Blue? from FiveThirtyEight](https://projects.fivethirtyeight.com/2016-swing-the-election/), [Undue Force from the Baltimore Sun](http://data.baltimoresun.com/news/police-settlements/) and [Spies in the Skies from BuzzFeed](https://www.buzzfeed.com/peteraldhous/spies-in-the-skies?utm_term=.hhenRxQPy1#.kgP31Xg2No) are built with custom code outside of the regular CMSs.) Knowing how to code that up is essential if you want to add interactivity to your story. 

⋅⋅*How to envision and code a small menu of CSS animations and jQuery elements. This is the fun stuff: transitions, scroll-based animations, reveals, hovers, etc. Ever wonder how [The Pudding](https://pudding.cool) works? We’ll get you started coding these little gizmos. 

*We all have different levels of experience with HTML, CSS and Javascript. The goal of this bootcamp is to get us all roughly on the same page.*

# Booting up a standalone webpage using Skeleton 

To layout an article, it helps to have a grid and a system to organize all your interconnected elements. In web design, this is called a framework. These frameworks are packages that structure your HTML, your CSS and other related elements like Javascript documents. Some frameworks you may have heard of: Bootstrap, Foundation, Groundwork, Gumby, and Skeleton. 

[Skeleton](http://getskeleton.com/), which is one of the most bare bones responsive frameworks out there, is what we'll be using for this workshop.

### Download Skeleton 

Download Skeleton, unzip it and open up the entire folder in a text editor like [Sublime Text 2](http://www.sublimetext.com/2). 

![img1](http://www.storybench.org/wp-content/uploads/2015/08/skeleton_html1-1440x760.png)

### Take a tour of the index page

Look for the `<html>, <head>, and <body>` tags.

### Add a title, description and author in the <head>

Take a look around and try to understand what all is being laid out in the `<head>` of your index.html page. Start by adding your title, description and author.

### Add a full-bleed hero image to the <body>

Paste in the following below the `<body>` tag. Link to a large image (ideally over 2,000 pixels wide) in `src=`.

```
  <!-- Hero image
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <div>
  <img class="u-full-width" src="http://aleszu.com/workshops/webdesign/images/publiceditors-cover.jpg" />
  </div>
```

### Add content to the <body> 

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

### Preview the page

Open the index.html from your Skeleton folder in a browser to preview the page you've been building.

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

### Adding a CSS animation

### Adding a jQuery element

### Adding a D3plus graphic





