---
layout: minimal
title: "How to Use"
date: 2016-05-08 20:35:48
image: '/assets/img/contribute.png'
description: 'How to contribute to robots.ros.org'
main-class: 'meta'
color: '#7AAB13'
tags:
- misc
- jekyll
categories:
twitter_text: 'How to use this template'
introduction: 'How to use this template'
---

# Goals

This site is designed to provide a showcase for robots using ROS.

## Who can contribute?

Anyone can contribute to the site. However it is expected that the majority of contributors are expecected to be the robot manufacturers or ROS integratoin maintainers.


## What content should be on the site?

This site is designed to be a portal for discovery and comparison of robots that publicly documented ROS interfaces.

Developer documentation should remain on the [ROS wiki](http://wiki.ros.org).
And pages on this site should not be the primary reference for a robot.
It should have it's own website with the majority of it's marketing and promotional content sales opportunities etc. 


## Featured Spotlight

Robots may be promoted to the spotlight on the home page.
To inquire about being promoted please contact  info@osrfoundation.org .

## How to contribute

To add a robot or make an update to the site, please [open a pull request on github](https://github.com/ros-infrastructure/robots.ros.org)

Documentation on how the site is setup can be found below.

## Guidelines for contributions

- Make sure to follow the tagging conventions.
- Do not spam the site with small variants of robot names. Only have one entry per major version, a model upgrade should not generate a new page.
- Keep the look and feel of the overall site, but feel free to customize within the framework.
- External javascript dependencies are generally discouraged but can be considered.



# About the backend

This site is bsased on the Cards Jekyll Template more information about the template is below.

## Cards Jekyll Template - [Demo](http://willianjusten.com.br/cards-jekyll-template)

This is a simple and minimalist template for Jekyll designed for developers that want to write blog posts but don't want to care about frontend stuff.

The Theme features:

- Gulp
- Stylus (Jeet, Rupture, Kouto Swiss)
- Live Search
- Offcanvas Menu
- SVG icons
- Very very small and fast!
- Shell Script to create posts
- Tags page
- Series page
- About Me page
- Feed RSS
- Sitemap.xml
- Color Customization
- Info Customization

## Basic Setup

1. [Install Jekyll](http://jekyllrb.com)
2. Fork the [Will Jekyll Template](https://github.com/willianjusten/will-jekyll-template/fork)
3. Clone the repo you just forked.
4. Edit `_config.yml` to personalize your site.
5. Check out the sample posts in `_posts` to see examples for assigning categories and tags, and other YAML data.
6. Read the documentation below for further customization pointers and documentation.
7. **Remember to compile your assets files with Gulp.**

## Site and User Settings

You have to fill some informations on `_config.yml` to customize your site.

```
# Site settings
description: A blog about lorem ipsum dolor sit amet
baseurl: "" # the subpath of your site, e.g. /blog/
url: "http://localhost:3000" # the base hostname & protocol for your site 

# User settings
username: Lorem Ipsum
user_description: Anon Developer at Lorem Ipsum Dolor
user_title: Anon Developer
email: anon@anon.com
twitter_username: lorem_ipsum
github_username:  lorem_ipsum
gplus_username:  lorem_ipsum
disqus_username: lorem_ipsum
```

## Header Name

To use the power of CSS Content and media query, the header name is defined on [src/styl/_header.styl](). Change to your prefered name.

## Color customization

All color variables are in `src/styl/variable`. To change the main color, just set the new value at `main` assignment. Another colors are for texts and the code background color.

## Theme Colors

Every post has a main color that is defined on [src/styl/_theme-colors.styl](). Just create a new color with the prefix `post-` and define your main-class: 'css' and color: '#2DA0C3' on every post you create.

## Creating posts

You can use the `initpost.sh` to create your new posts. Just follow the command:

```
./initpost.sh -c Post Title
```

The new file will be created at `_posts` with this format `date-title.md`.

## Front-matter 

When you create a new post, you need to fill the post information in the front-matter, follow this example:

```
---
layout: post
title: "Falando sobre RSCSS"
date: 2016-02-07 18:48:16
image: '/assets/img/rscss/rscss.png'
description: 'Escrevendo CSS sem perder a sanidade. Aprenda uma metodologia que pode salvar muitas dores de cabeça.'
main-class: 'css'
color: '#2DA0C3'
tags:
- css
- metodologia
- frontend
categories:
twitter_text: 'Escrevendo CSS sem perder a sanidade.'
introduction: 'Escrevendo CSS sem perder a sanidade. Com essa introdução, Rico St. Cruz o criador chama a atenção de todos sobre uma metodologia melhor para se escrever CSS.'
---
```

## Running the blog in local

In order to compile the assets and run Jekyll on local you need to follow those steps:

- Install [NodeJS](https://nodejs.org/)
- Run `npm install` 
- Run `gulp`

## Windows 10 Step

If you use Windows 10, change this line on [gulpfile.js](https://github.com/willianjusten/will-jekyll-template/blob/gh-pages/gulpfile.js#L23) to `spawn('jekyll.bat', ['build'])`.

## Questions

Having a problem getting something to work or want to know why I setup something in a certain way? Ping me on Twitter [@willian_justen](https://twitter.com/willian_justen) or file a [GitHub Issue](https://github.com/willianjusten/will-jekyll-template/issues/new).


## Donation

If you liked my work, buy me a coffee <3

[![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=UTMFZUHX6EUGE)

## License

This theme is free and open source software, distributed under the The MIT License. So feel free to use this Jekyll theme on your site without linking back to me or using a disclaimer.

If you’d like to give me credit somewhere on your blog or tweet a shout out to [@willian_justen](https://twitter.com/willian_justen), that would be pretty sweet.
