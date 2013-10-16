Hub CMS
=======

What Is Hub CMS?
----------------

Hub CMS is an actual CONTENT management system. Most CMSs are really web site management systems. Yes, you create content, but it’s really only meant for the web. It can work on a mobile device if you use a responsive theme.

Hub CMS strives to live up to the ideal of truly [adaptive content](http://karenmcgrane.com/2012/09/04/adapting-ourselves-to-adaptive-content-video-slides-and-transcript-oh-my/). You create/assemble the content in all its parts and pieces: text, images, audio, video, files, etc. That content is made available through an API, and it’s up to other software to do with that content as it sees fit: a website builder, an iPhone app, an Android app, a script, a program,  etc. It’s true separation of content from presentation.

Hub is also an automated content distribution system.

Content is not usually just a lone piece of text, or just one single image. It needs to be grouped together in relevent ways.

Let's use a talk at [Laracon](http://laracon.eu/2013/) for an example. [Taylor Otwell](https://github.com/taylorotwell) gives a presentation. By the end, the following pieces of content, getting more elaborate as we go, could be available:

1. A short string of text containing the title
1. The date and timestamp of the talk
1. The duration of the presentation
1. Biographical info about Mr. Otwell
1. A short teaser description of what the talk is about
1. Tags to categorize the talk
2. The event he spoke at
1. A video of his talk
1. An audio only recording
1. A text transcript
1. Slides that were up on the screen
1. A PDF file of the handout given to accomapny the presentation
1. Code fragments used in examples
1. A series of photos, both of Mr. Otwell, and the audiance sitting on the edge of their seats
1. A list of links to sources referenced
1. Survey results from audiance feedback
2. Comments posted after the talk
1. Tweets with related hashtags made during the talk
1. Geotag data of where the talk was held
1. Who knows what else...

This is all grouped together as related data for a single presentation or talk.

Phew! We've got all this data, now what do we do with it? We C.O.P.E. Cope? It's a lot of data, but it's not that traumatic an experience! No, C.O.P.E. stands for Create Once, Publish Everywhere.

We can do anything we - legally - want with this content, and we get the computer to do what computers do best: automate. Yes, the API is available to grab information on demand. If a service needs to check once a day for updates, it can do that. But that's old school. The real power comes from pushing content out for distribution.

Some of these examples are all ready very possible with current software and APIs. Others may be possible in the future. Some of it may just be dreaming.

Let's start with a common need: using this data to create a webpage. We inform the web publishing platform there is new content to be had. It grabs the pieces it actually wants, caches it so it's not hounding the core on every page view. The data is then assembled into a web page about this one presentation, and listed in the index along with other talks. The tags are added to the tag cloud, and the author's bio is shown too. There's a link to download the PDF and also a way to view the slides.

We've have a shiney HD video file uploaded. Now we can automatically copy it to our cloud file server. It's also automatically uploaded to YouTube, along with tags and description; perhaps other supported video sites as well. When the video is ready for the public, we update our data with video links. We then tell our web publisher there's been an update. It changes the page to now include the embedded YouTube video.

Audio could be automatically extracted from the video, converted to various formats, and distributed to audio sharing sites. The web platform could be informed, and then include ways to listen right on the website, as well as download.

A copy of the audio is sent to whomever is responsible for typing out the transcript. They do their thing, then submit their work. When approved, its now available for use. It can be sent to YouTube for it to turn into captions, added to the webpage, and turned into a PDF for download.

The photos can be uploaded to Facebook and Flickr. One of them can be used as a thumbnail for the talk. All of them can be displayed on the website as a slideshow.

The code gets pushed to GitHub, then the link to its repository added to the metadata for the talk. The web page updates with a nice button link.

Meanwhile the native smartphone apps are updating too, displaying just what's needed, made to look good on small screens and designed for touch.

It might be silly for the website and mobile apps to update piecemeal, so maybe things are set so the content is only a draft until all the important pieces are in place, then push out.

Meanwhile the RSS feed is updated, an email is sent out to subscribers, and the conference Twitter and Facebook feeds get updates.

Somewhere down the road, all the videos are sent to a company who makes a DVD set to be sold. The transcripts get turned into an ebook.

And on and on it goes. The point is you put content in one place, then automate all sorts of things, and distribute that content everywhere that's relevent as fast as possible.

Yes, custom solutions have been made to do things like this. The goal here is to make a system easy enough and flexible enough that practically anyone can create all kinds of useful content groups, or objects, and the distribution automation to go with it. For more advanced needs, coders can open their editors and make a plugin.

The example used is in no way meant to imply an endoresement from anyone. I used the example because Hub will make strong use of the [Laravel PHP framework](http://laravel.com/), and Taylor Otwell is sure to give a talk because he's the man who started Laravel. And he's awesome.

To Do
-----
* Everything. This is just an idea right now.
* Write a clearer, shorter description. Challenging, as this is different than what most people are used to. Pictures might help.
* Slow down. My imagination may well outweigh my ambition.
