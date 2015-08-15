# ...know when a new version is released? #

Subscribe to the Downloads RSS feed which is one of the <a href='http://code.google.com/p/restylegc/feeds'>many that are available</a>.

# ...change the background color? #

  1. Make sure to remove the inline style from the body tag.  This is accomplished by:
```
    $('body').removeAttr('style');
```
> > and should already be present.
  1. Add a `background` or `background-color` property to the `body` style block.
  1. Make sure to add `allowtransparency="true"` to the `<iframe>` tag.  This is necessary for IE to display the background color properly.

# ...change the calendar images? #

The majority of the images are now contained in a single sprite sheet named, for example, `combined_v7.gif`. In previous versions, the images were separated into individual files.

  1. Download the latest sprite sheet from Google.
  1. Edit the file.
  1. Change all references in the stylesheet to point to your version, instead of the one from Google.  Typically, they will look like:
```
  background-image: url(//calendar.google.com/googlecalendar/images/combined_v7.gif);
```
  1. Some images still are individual files, for example, the print icon.  Those should already point to the file in the `images` folder, so you should be able to edit it, and the change should be immediately visible.

# ...display a specific date or date range? #

<strike>There is an undocumented feature of Google Calendar that allows you to specify a date range.  Add the following variable to your query string:<br>
<pre><code>dates=YYYYMMDD%2fYYYYMMDD<br>
</code></pre>
where YYYYMMDD represents a date as Year-Month-Day.  This is most useful when the mode is set to agenda, and you want to display future events and not just the current month's events.</strike>

This technique does not appear to work anymore.


# ...remove the Google logo? #

Personally, I don't think you should do this, but here are the instructions anyway.

  1. Add `display:none` to the `.subscribe-image` style block.

