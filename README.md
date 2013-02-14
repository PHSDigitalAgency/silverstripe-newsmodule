# silverstripe-newsmodule
=======================

## Introduction

This is the Silverstripe 3 Newsmodule. It's a very basic newsmodule, separate from the SiteTree.
Mainly to keep the SiteTree uncluttered. 

It works. Pretty much. Has some missing features. Please read my comments on the functions and such. It should make everything clear.
If it doesn't... Then... wait a bit until I update this, ok?

Ow, and the default template is based on HTML5 features and my own website. Functional frontend demo can also be found on my website. `http://casa-laguna.net/all-the-news`

Strange code and undocumented features are probably due to my cat sleeping on the keyboard.

I strongly advice to read my inline comments. I've worked hard to make them both functional as funny. Feedback appreciated.
And keep an eye on my issues, those are issues I want to fix or features I want to add. Feel free to add suggestions!

## Maintainer Contacts

* Simon "Sphere" Erkelens `simon[at]casa-laguna[dot]net`

## Features

* Handle news and impressions besides the news.
* Support for OG-data on some servers (some servers refuse for some reason). Check here for the OG-module: `https://github.com/tractorcow/silverstripe-opengraph`
* History of URL-segments.
* Support for custom comments.
* Akismet support.
* Globally available NewsArchive function.
* Configurable from the SiteConfig.
* GridField overview, less clutter in the SiteTree.
* RSS Feed, can be found under `http://yoursite.com/yournewspage/rss` (Note, it seems links in content are not parsed correctly in the RSS-entry builder!)
* If you include and setup my [`Silverstripe Social`](https://github.com/Firesphere/silverstripe-social) you can make it auto-post new items to Twitter

## Lacks

* History of changes in the items
* 

(Indeed, that second bullet means it only lacks history, nothing else :P )

## Installation

If you don't have a github account, just download:
 1. Click on the big "ZIP" button at the top.
 2. Extract the zip to your site-root
 3. Run in your browser - `www.example.com/dev/build` to rebuild the database. 
 4. Create a NewsHolderPage type in your Pages Admin (todo, autocreate this page)

Other option is to clone the repo into your site-root:
 1.  In your site-root, do `git clone https://github.com/Firesphere/silverstripe-newsmodule.git`. 
 2.  Run in your browser - `www.example.com/dev/build` to rebuild the database. 
 3.  Create a NewsHolderPage type in your Pages Admin (todo, autocreate this page)

Although, I would like it if you forked and cloned, because if you do, you can help me by adding features and make pull-requests to improve this module!
 1.  Make a fork of this module.
 2.  In your site-root, do `git clone https://{your username}@github.com/{your username}/silverstripe-newsmodule.git`. 
 3.  Run in your browser - `www.example.com/dev/build` to rebuild the database. 
 4.  Create a NewsHolderPage type in your Pages Admin (todo, autocreate this page)

Note, forking is NOT REQUIRED, only handy if you want to help out.

## Best Practices

* Write grammatically correct.
* If you have Akismet, add your Akismet API-key to _config.php as exampled. It saves you from comment-spam

## Configuration

* In the SiteConfig, set your wished configuration in the News-tab.

## Plans

* Integrate Facebook OAuth to automagically post when a new item is created.
* Add a slideshow feature. Currently, not available, but you can use your own by integrating a slideshow manually.
* Add smiley/BB-code support to comments and items.
* Add a "Fetch me a beer" function. Should be useful I think.
* Implement what I wrote here: `http://casa-laguna.net/all-the-news/show/geshi-and-tweet-rendering-in-silverstripe`
* More to come, but I can't think of it right now :(

## Known Issues

* The MD5-Email field, required if you want Gravatar-support, is named "MD5Comment". Don't ask.
* The Impression is at the top. It should be at the bottom. I haven't looked into that yet.
* RSS Feed is breaking content-links!

## Requests

* Improvements.
* Translations.

## Other

* This module is given "as is" and I am not responsible for any damage it might do to your brain, dog, cat, house, computer or website.
* Code Comments should not be taken too seriously, since I'm bad at writing serious code-comments.
* Please use the Issue-tracker, otherwise I get lost too.
* This ModelAdmin method is chosen to declutter the SiteTree.
* This is a port of a non-released SS2.4 newsmodule I wrote. It might not be entirely "up to code" yet.

## Actual license

This module is published under BSD 2-clause license, although these are not in the actual classes, the license does apply:

http://www.opensource.org/licenses/BSD-2-Clause

Copyright (c) 2013, Simon "Sphere" Erkelens

All rights reserved.

Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:

    Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
    Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.


(I shouldn't scream, should I? This is copy-paste from BSD-2 license...)
