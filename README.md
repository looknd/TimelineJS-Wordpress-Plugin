# TimelineJS 
## Document history with TimelineJS
Contributors: miguelpeixe, zachwise
Tags: timeline, shortcode, stamen, timeline.verite.co, VeriteCo, HTML5
Requires at least: 2.0.2
Tested up to: 3.3.2
Stable tag: 2.11.1

Use TimelineJS developed by VéritéCo for your Wordpress site. As easy as writing a shortcode.

## Description

There are lots of timeline tools on the web but they are almost all either
hard on the eyes or hard to use. Create timelines that are at the same time
beautiful and intuitive for users

TimelineJS is great for pulling in media from different sources. Just throw in a
link from Twitter, YouTube, Flickr, Vimeo, Google Maps or SoundCloud and
TimelineJS will format it to fit perfectly. More media types will be supported
in the future.

Creating one is as easy as filling in a Google spreadsheet or as detailed as
JSON.

A simple shortcode plugin to add the TimelineJS made by [VéritéCo](http://verite.co/).
To embed your timeline use the button located at the post content editor (TinyMCE).

**You can also embed the Timeline on your post using this shortcode :**
`[timeline src="Your source url here"]`

**TIP** - If you want to embed outside of a post, use the following code:
`<?php echo do_shortcode('[timeline src="Your source url here"]'); ?>`


## Installation

1. Upload the plugin to the `/wp-content/plugins/` directory
1. Activate the plugin through the 'Plugins' menu in WordPress
1. Learn how to create the TimelineJS source at http://timeline.verite.co/#fileformat
1. Use the shortcode on your post/page: `[timeline src="Your source url here"]`

**Extra tip** - If you want do embed outside of a post, use the following code on your template:
`<?php echo do_shortcode('[timeline src="Your source url here"]'); ?>`

## File Formats

### Google Docs:

If you don’t want to mess with JSON, fire up Google Docs and build your
timeline in a spreadsheet. It’s as simple as dropping a date, text, and links
into the appropriate columns in TimelineJS’s template.

You can find the template here: [TimelineJS Google Spreadsheet Template](https://docs.google.com/a/digitalartwork.net/previewtemplate?id=0AppSVxABhnltdEhzQjQ4MlpOaldjTmZLclQxQWFTOUE&mode=public)

There are only a couple things you need to know in order to create a timeline
using Google Docs:

  1. Make the spreadsheet public:   
	Google Docs are automatically set to private but the spreadsheet must be
	public.
	
	Click the blue “Share” button on the top right-hand corner. In the “Share
	settings” window, you’ll see the private setting of the spreadsheet: click
	“Change...”. In the Visibility options window, choose “Public on the Web” and
	save.

  2. Publish to the Web  
	Under the File menu, select “Publish to the Web.”
	
	In the next window, check the box next to “Automatically republish when
	changes are made.” Uncheck all other boxes. Click “start publishing.” This
	will give you the URL to embed in your HTML file.

  3. Copy/paste the Web URL into your TimelineJS HTML file  
	After you publish the spreadsheet, Google Docs will generate a link to the
	file. Copy the link for the Web Page option (as opposed to PDF, HTML, XLS,
	etc.), then paste it into the timeline’s HTML file (see [Add it to your site](#add-it-to-your-site) )


## Shortcode Options
Here are some of the options you can set in the config.

### Language
`lang`
Localization
*default is en*
Languages available:
* `en` *English*
* `fr` *Français*
* `es` *Español*
* `de` *Deutsch*
* `it` *Italiano*
* `pt-br` *Português Brazil*
* `pt` *Português*
* `nl` *Dutch*
* `cz` *Czech*
* `dk` *Danish*
* `id` *Indonesian*
* `pl` *Polish*
* `sl` *Slovenian*
* `ru` *Russian*
* `sk` *Slovak*
* `is` *Icelandic*
* `fo` *Faroese*
* `kr` *월요일*
* `ja` *日本語*
* `zh-ch` *中文*
* `zh-tw` *Taiwanese Mandarin*
* `ta` *தமிழ் - Tamil*
* `ar` *Arabic* *May be issues with right to left (need some help here)* 

Help us add more. Grab a copy of a language file and replace it with your language [Example language file](https://github.com/VeriteCo/StoryJS-Core/blob/master/Language/locale/en.js) and find your language's [two letter code here](http://spreadsheets.google.com/pub?key=p9pdwsai2hDMsLkXsoM05KQ&gid=1)

###Start at End 
`start_at_end`
set to true to start the timeline on the last date.
*default is false*

###Start at Slide 
`start_at_slide`
You can tell TimelineJS to start at a specific slide number
*default is 0*

###Start Zoom Adjust
`start_zoom_adjust`
This will tweak the default zoom level. Equivilent to pressing the zoom in or zoom out button the specified number of times. Negative numbers zoom out.
*default is 0*

###Hash Bookmark 
`hash_bookmark`
set to true to allow bookmarking slides using the hash tag
*default is false*

###Debug 
`debug`
Will log events etc to the console.
*default is false*


###Map Style Types 
Due to recent changes to the Google Maps API, you need a [API Key](https://developers.google.com/places/documentation/#Authentication) in order to use custom map types.
`gmap_key:`
*required in order to use maptype*

`maptype:`
* [Stamen Maps ](maps.stamen.com)
* `toner`
* `toner-lines`
* `toner-labels`
* `watercolor`
* `sterrain`
		
* Google Maps
* `ROADMAP`
* `TERRAIN`
* `HYBRID`
* `SATELLITE`

###Font Options 
`font:`
* `Arvo-PTSans`
* `Merriweather-NewsCycle`
* `PoiretOne-Molengo`
* `PTSerif-PTSans`
* `DroidSerif-DroidSans`
* `Lekton-Molengo`
* `NixieOne-Ledger`
* `AbrilFatface-Average`
* `PlayfairDisplay-Muli`
* `Rancho-Gudea`
* `Bevan-PotanoSans`
* `BreeSerif-OpenSans`
* `SansitaOne-Kameron`
* `Pacifico-Arimo`
* Or make your own

####Font Combination Preview:
![Font Combination Preview](http://timeline.verite.co/gfx/font-options.png)
  
  
## Changelog
### 2.11.1 ###
* Update Timeline to the latest version

### 0.9.7 ###
* Update Timeline to the latest version

### 0.9.6 ###
* Update Timeline to the latest version

### 0.9.5 ###
* Update Timeline to the latest version

### 0.9.4 ###
* Local storing Timeline files
* Adding more map style options for TinyMCE

### 0.9.3 ###
* l18n support for TinyMCE
* Brazilian Portuguese translation for TinyMCE

### 0.9.2 ###
* Added TinyMCE button

### 0.9.1 ###
* Small bugfix for default width/height

### 0.9 ###
* Language support based on WordPress locale:
  * Brazilian Portuguese
  * French
  * Spanish
  * German - Deutsch
  * Italian
  * Korean
  * Chinese
  * Taiwanese

### 0.8 ###
* First stable release.
