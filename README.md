## Links

- [Changelog](https://todo.syncforreddit.com/changelog)
- [Discord](https://discord.gg/sync-for-reddit)
- [Subreddit](https://reddit.com/r/redditsync)

## Work in progress

	### Profiles
		- Design new comment slide holder
		- hook up profiles chip bar
		- Check profile bottom sheet

	### Drawer
		- Add in account changer

	### Comments
		- Update comment search to use the new design
		- Move comments notification bar (archive etc) out of the app bar
	
	### Chipbar
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

## TODO

### Refactoring
	- Check what is still using legacy activity
	- Go through and remove any calls to the old HTML to Spannable parser
	- Remove any references to ColorUtil.isColorDark (should just be using the palette now)
	- ColorUtils.setAlphaComponent
	- Delete custom positive button and negative button (use the new component)
	- Delete ClickableMovementMethod, CustomUrlSpan, LongClickLinkMovementMethod
	- Ensure we're not using any outline providers still

### Posts
	- Make sure the divider is still working

### Messaging
	- Setup new views for messaging
	- Need to set the target ID for messaging header
	- Messaging padding at top too large

### Slides
	- Hook up comment slides

### Cards
	- Hook up the new inline video player for cards	
	- Add the new pinned posts header

### Posts 
	- Update post adapter to use the UI mode
	- Optimise the post adapter

### Basics
	- Hook up messaging
	- Hook up moderator
	
### New toolbar
	- Add droop down to the small toolbar
	- Decide what to do with the large header on click

### Important
	- Fix all the flags to add | PendingIntent.FLAG_IMMUTABLE

### Bugs
	- Nav bar not fully hiding when scrolling
	- Volume indicator broken on inline gifs
	- Post opening ripple effect broken on oneplus
	- Missing favicons
	- Search in settings has a bugged toolbar

### Known issues
	- Dividers arent shown inbetween comments in the comment search bottomsheet

### Internal
	- Delete SelftextCardView
	- Test share image of slide
	- Remove LegacyCustomImageView
	- Delete slideimagewrapper
	- Revisit how missing thumbnails are generated
	- Fix swipe mode
	- Animated emotes

### Small issues
	- Remove any references to the old save logo

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
	- Should Sidebar should comeback as a sidebar?
	- Links are no longer underlined. Thoughts?

### Onboarding ideas
	- Select flair display type
	- Select award display type