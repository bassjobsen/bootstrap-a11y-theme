Bootstrap a11y theme
====================

How to Compile your CSS
-----------------------

Recompile Bootstrap:

 - copy a11y.less to your Bootstrap's LESS folder
 - add `@import "a11y.less";` at the end of booststrap.less
 - recompile Bootstrap
 
Compile the theme:
 - copy a11y.less and a11ytheme.less to your Bootstrap's LESS folder
 - recompile your theme: `lessc a11ytheme.less > a11ytheme.css`
 
You can also download [a11ytheme.css](https://github.com/bassjobsen/bootstrap-a11y-theme/blob/master/a11ytheme.css) or [a11ytheme.min.css](https://github.com/bassjobsen/bootstrap-a11y-theme/blob/master/a11ytheme.min.css) from this site.

How to use the theme's CSS
--------------------------

You can't use the theme without Bootstrap's CSS, so use:

    <link href="//netdna.bootstrapcdn.com/bootstrap/3.1.1/css/bootstrap.min.css" rel="stylesheet">
    <link href="a11ytheme.min.css" rel="stylesheet">


NB if you recompiled Bootstrap, you only will need the recompiled CSS.

Also try the [Bootstrap Accessibility Plugin](http://paypal.github.io/bootstrap-accessibility-plugin/), This plugin adds accessibility mark-up to the default components of Bootstrap 3 to make them accessible for keyboard and screen reader users.

HTML
----

Add a ` <a class="sr-only" href="#content">Skip to content</a>` link to your navbar:

	<nav class="navbar navbar-default" role="navigation">
		<a class="sr-only" href="#content">Skip to content</a>	
		  <div class="container-fluid">
			<div class="navbar-header">
			  <button type="button" class="navbar-toggle" data-toggle="collapse" data-target=".navbar-collapse">
				<span class="sr-only">Toggle navigation</span>
				<span class="icon-bar"></span>
				<span class="icon-bar"></span>
				<span class="icon-bar"></span>
			  </button>
			</div>
				<div class="collapse navbar-collapse" id="bs-example-navbar-collapse-1">
				  <form class="navbar-form navbar-left" role="search">
					<div class="form-group">
					  <input type="text" class="form-control" placeholder="Search">
					</div>
					<button type="submit" class="btn btn-default">Submit</button>
				  </form>
				</div> 
			
		  </div>
	</nav>

Demo
----
You can visit [Bootstrap a11y theme's style guide](http://jbst.eu/bootstrap-a11y-theme/).

What does Bootstrap a11y theme's fix?
-------------------------------------

 - replace the screen readers only CSS
 - adds 'skip to content' link
 - match color contrasts
 - font sizes to match color contrasts
 
JBST
----
This theme is initial written for [JBST](http://jbst.eu/). JBST is a powerful theme framework for WordPress that can be used as a standalone website builder or as a framework to create child themes for WordPress. JBST build on the top of Twitter's Bootstrap 3 and is full customizable with LESS. Integrated customizer for easy responsive website building. Right-To-Left (RTL) support. It also has built in support for BuddyPress, BBpress and eCommerce (WooCommerce, JigoShop and WPeCommerce). Without this theme JBST didn't meet [Wordpress.org's guidelines for accessibility] (http://make.wordpress.org/themes/guidelines/guidelines-accessibility/).
 
About Bootstrap
---------------
[Bootstrap](http://getbootstrap.com/) is the most popular front-end framework for developing responsive, mobile first projects on the web.
 
About a11y (web accessibility)
------------------------------
 
 - [The Accessibility Project](http://a11yproject.com/), A community-driven effort to make web accessibility easier.
 - [Web Accessibility for Designers](http://webaim.org/resources/designers/)
 
Tools:
 
 - [/ContrastA](http://www.dasplankton.de/ContrastA/), Find Accessible Color Combinations

 
 
