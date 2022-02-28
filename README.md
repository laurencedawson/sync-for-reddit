## Links

- [TODO](https://todo.syncforreddit.com)
- [Changelog](https://todo.syncforreddit.com/changelog)
- [Beta discussion](https://todo.syncforreddit.com/discussion)

## Work in progress

	### Important
		- Fix all the flags to add | PendingIntent.FLAG_IMMUTABLE

	### Messaging
		- Setup new views for messaging
		- Need to set the target ID for messaging header
		- Messaging padding at top too large

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
	- Delete ProfileBottomSheetFragment
	- Check what is still using legacy activity
	- Go through and remove any calls to the old HTML to Spannable parser
	- Remove any references to ColorUtil.isColorDark (should just be using the palette now)
	- ColorUtils.setAlphaComponent
	- Delete custom positive button and negative button (use the new component)
	- Delete ClickableMovementMethod, CustomUrlSpan, LongClickLinkMovementMethod
	- Ensure we're not using any outline providers still
	- Remove all final references to the old theme manager (StyleSingleton)
	- Remove all saved settings for the old theme
	- Look into changing the ripple drawable everywhere

### Cards
	- Hook up the new inline video player for cards	
	- Add the new pinned posts header

### Posts 
	- Update post adapter to use the UI mode
	- Optimise the post adapter
	- Hook up and test alt post types

### Basics
	- Hook up moderator
	
### New toolbar
	- Add droop down to the small toolbar
	- Decide what to do with the large header on click

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