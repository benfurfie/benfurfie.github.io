---
layout: "post-sidebar"
published: true
comments: true
read_time: "The WP JSON API isn't scary"
modified: ""
author_name: Ben Furfie
author_url: /author/ben
author_avatar: ben
categories: 
  - WordPress
feature_image: ""
square_related: ""
title: "Think the WP REST API is scary? Think again..."
---

The last 12 months have seen a huge amount of buzz in the WordPress community about the introduction of the REST API.

That buzz went through the roof over the weekend after Matt Mullenweg in his State of the Word talk at WordCamp US dropped the strongest hint yet that the future of WordPress was written in Javascript.

I was lucky enough to see Jack Lenox's talk about [building themes with the WordPress API](http://jacklenox.com/2015/03/30/building-themes-with-the-wp-rest-api-wordcamp-london-march-2015/) at WordCamp London back in March this year. Ever since then, I've been hankering to get my teeth into playing with the WP REST API.

However, since then I shuttered my freelance business and went in house at a major Drupal agency. One of the reasons I was hired was to help drive the introduction of WordPress into the business – and now that I feel comfortable with Drupal – I've been increasingly able to turn my attention back to WordPress.

## The REST API isn't that scary... honest
If you're a web developer or implementor who build their first website using WordPress and has never ventured outside the world of themes, learning Javascript can be quite an intimidating idea – especially considering the pain many aspiring developers go through learning PHP.

So it's unsurprising that many have expressed fear at the prospect of having to learn another, equally-technical language like Javascript.

I had a couple of hours free this evening and so decided to have a quick play around with the REST API and see how simple it really is to get started with it.

Here's what you'll need:
- A basic understanding of Javascript and jQuery (in particular variables)
- A local development environment (I use MAMP Pro as I work with more than just WordPress. But if your primary – or only – CMS is WordPress, go checkout DesktopServer)
- The JSON API plugin (unless WordPress 4.4 is out, which comes with it baked in).

## First things first – what is JSON
I won't go into the technicalities of what JSON is or how it works. All you need to know is that it stands for **J**ava**S**cript **O**bject **N**otation and that it's a way of parsing data in a way that makes it easy to share between servers and websites.

## Setting up
You'll need to create two different websites – one that is a WordPress website and another that is a static HTML website (which is where the magic will happen).

Set up your WordPress website as you would normally (if you're new to local development, I'd suggest checking out [Treehouse](http://www.teamtreehouse.com) or [Lynda](http://www.lynda.com) – they've got some great courses on local development specific to WordPress).

On your WordPress site, don't worry about the theme that is active – you won't be using it. Instead, go to plugins and install the JSON API plugin (you can find it in the WordPress plugin repo).

_Note: If you have WordPress 4.4 or later installed, you can skip this step as the JSON API comes baked in._

Once you have done that, you're finished with that site as we'll be working with the dummy content. (Once you've finished with this, by all means go back and add more content to play around with this example.)

Now go and set up your static website and create a file called _index.html_. You'll also want to create a folder called _public_ and a file in it called _controller.js_.

### index.html
Open up index.html in a code editor and paste the following code:

<script src="https://gist.github.com/benfurfie/ce28f6153cb6453c84e2.js"></script>

If you're at all familar with the web, you should recognise most of this code.


