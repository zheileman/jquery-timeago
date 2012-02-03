# Please note: changes introduced in this fork:

1) **Use 'data-time' attribute instead of the 'title' attribute for storing the ISO 8601 timestamp.**

2) **New configuration setting to enable/disable overwriting 'title' attribute with the tag content (defaults to false)**

3) **Updates to this README to reflect the changes**

# timeago: a jQuery plugin

Timeago is a jQuery plugin that makes it easy to support automatically updating
fuzzy timestamps (e.g. "4 minutes ago" or "about 1 day ago") from ISO 8601
formatted dates and times embedded in your HTML (à la microformats).

## Usage

First, load jQuery and the plugin:

```html
<script src="jquery.min.js" type="text/javascript"></script>
<script src="jquery.timeago.js" type="text/javascript"></script>
```

Now, let's attach it to your timestamps on DOM ready:

```html
<pre>
   jQuery(document).ready(function() {
     jQuery("abbr.timeago").timeago();
   });
</pre>
```

This will turn all abbr elements with a class of timeago and an ISO 8601 timestamp in the title:

```html
<abbr class="timeago" data-time="2008-07-17T09:24:17Z">July 17, 2008</abbr>
```

into something like this:

```html
<abbr class="timeago" data-time="2008-07-17T09:24:17Z" title="July 17, 2008">about 1 day ago</abbr>
```

or, when title is disabled in settings (in case you don't want tooltips):

```html
<abbr class="timeago" data-time="2008-07-17T09:24:17Z">about 1 day ago</abbr>
```

As time passes, the timestamps will automatically update.

**For more usage and examples**: [http://timeago.yarp.com/](http://timeago.yarp.com/)

**For different language configurations**: [http://gist.github.com/6251](http://gist.github.com/6251)

## Author

[Ryan McGeary](http://ryan.mcgeary.org) ([@rmm5t](http://twitter.com/rmm5t))
Fork by [Jesus L. / Zheileman](http://jesuslaiz.com)

## Other

[MIT License](http://www.opensource.org/licenses/mit-license.php)

Copyright (c) 2008-2010, Ryan McGeary (ryanonjavascript -[at]- mcgeary [*dot*] org)
