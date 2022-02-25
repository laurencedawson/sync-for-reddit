## Links

- [Changelog](https://todo.syncforreddit.com/changelog)
- [Discord](https://discord.gg/sync-for-reddit)
- [Subreddit](https://reddit.com/r/redditsync)

## Work in progress

	### Drawer
		- Add in account changer

	### Misc
		- Delete custom positive button and negative button (use the new component)

	### Profiles
		- Design new comment slide holder

	- Update comment search to use the new design
	- Update search bottomsheet to use the new design

	- Hook up new chipbar!!
		- ~~Defaults~~
		- ~~Subreddits~~
		- ~~Multi~~
		- ~~Friends~~
		- ~~Search~~
		- ~~Watching~~
		- ~~Domain~~
		- ~~Seen~~
		- Profile
		- Mod
		- Messaging
		- Split section back up...

	- Check what is still using legacy activity
	- Update style for material dialogs

	- Work on switching over to Monet
	- Remove ColorUtil.isColorDark
	- ColorUtils.setAlphaComponent

	- Chipbar for comments
	- Volume indicator broken on inline gifs

	- Revert minimal awards are now the default
	- Revert minimal post flair is now the default


## TODO

### Posts
	- Make sure the divider is still working

### Messaging
	- Setup new views for messaging
	- Need to set the target ID for messaging header
	- Messaging padding at top too large

### Chips
	- Hook up "Top growing"

### Slides
	- Hook up comment slides
	- Selftext preview text size (seems to be different in the list than comments)

### Cards
	- Hook up the new inline video player for cards	
	- Add the new pinned posts header

### Settings
	- Update the toolbar colour

### Posts 
	- Update post adapter to use the UI mode
	- Optimise the post adapter
	- Update icon in CasualActivity to be "up"

### Basics
	- Hook up messaging
	- Hook up moderator
	- Hook up profiles
	
### New toolbar
	- Add droop down to the small toolbar
	- Decide what to do with the large header on click

### Important
	- Fix all the flags to add | PendingIntent.FLAG_IMMUTABLE

### Paused
	- Sidebar should comeback as a sidebar
	- Check profile bottom sheet

### Bugs
	- Nav bar not fully hiding when scrolling
	- About from picker broken

### Known issues
	- Dividers arent shown inbetween comments in the comment search bottomsheet

### Internal
	- Delete SelftextCardView
	- Test share image of slide
	- Remove LegacyCustomImageView
	- Delete slideimagewrapper
	- Revisit how missing thumbnails are generated
	- Fix swipe mode
	- Move comments notification bar (archive etc) out of the app bar
	- Animated emotes

### Small issues
	- Remove any references to the old save logo

### Monet
	- Add additional theming options

### Post launch
	- New app icon
	- Check that analytics is working right...
	- Enable play store install checker 
	- Enable crashlytics for releases
	- Look into adding headers with merge adapter
	- Monitor System.err

### To discuss
	- If a user has drawer disabled, where should the profile pic go?
	- What chips can be shown at the top of frontpage and all?
	- Need a clear way to show the default subreddit
	- Where to start autoplaying videos
	- How to expand the "refine" section under themes