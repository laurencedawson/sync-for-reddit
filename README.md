## Links

- [Changelog](https://todo.syncforreddit.com/changelog)
- [Discord](https://discord.gg/sync-for-reddit)
- [Subreddit](https://reddit.com/r/redditsync)

## Work in progress

	- Hook up new chipbar!!	
	- Chipbar for comments
	- Fix InlineImageSpan & EmoteImageSpan (also in CustomTextview)
	- ImageSpanUtils
	- Volume indicator broken on inline gifs

## TODO

### Chips
	- Hook up "Top growing"

### Slides
	- 

### Cards
	- Hook up the new inline video player for cards

### Settings
	- Update the toolbar cooler

### Posts 
	- Update post adapter to use the UI mode
	- Optimise the post adapter
	- Update icon in CasualActivity to be "up"

### Monet
	- Build a new theme manager
	- Hook up night mode
	- SelftextPreviewHolder needs updating to Monet
	- Add a new section to themes "Content highlight color"

### Basics
	- Hook up messaging
	- Hook up moderator
	- Hook up profiles

### Performance
	- Switch videos to their own view type
	- Unify SubView and ProfileView
	
### New toolbar
	- Add droop down to the small toolbar
	- Decide what to do with the large header on click

### Comments
	- 

### Drawer
	- Add in night mode changer to the drawer

### Drawer
	- Add in account changer

### Important
	- Fix all the flags to add | PendingIntent.FLAG_IMMUTABLE

### Paused
	- Add animation when showing the collapsed toolbar (maybe a fade)
	- Sidebar should comeback as a sidebar
	- Check profile bottom sheet

### Known issues
	- Toolbar icons don't work when collapses (disable join chip)
	- Toolbar icons mess up when changing theme

### Internal
	- Delete SelftextCardView
	- Test share image of slide
	- Revert minimal awards are now the default
	- Revert minimal post flair is now the default
	- Remove LegacyCustomImageView
	- Delete slideimagewrapper
	- Revisit how missing thumbnails are generated
	- Fix swipe mode
	- check share looks good
	- Check if streamable posts are considered video
	- Switching between night and day is flickering
	- Remove all instances of Picasso
	- Awards and flair wrapper still slow (maybe crashing too)

### Post launch
	- New app icon
	- Check that analytics is working right...
	- Enable play store install checker 
	- Enable crashlytics for releases
	- Look into adding headers with merge adapter
	- Monitor System.err