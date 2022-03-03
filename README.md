## Links

- [TODO](https://todo.syncforreddit.com)
- [Changelog](https://todo.syncforreddit.com/Changelog)
- [Beta discussion](https://todo.syncforreddit.com/discussion)

## Work in progress

### View types
	- Cards missing thumbnail not showing at all (cards)
	- test messages under different view types
	- add bit in settings to change view type



- Icons for user, OP, friend
- add option to move position of image for slide

- Sidebar...
- AMOLED
- Monet more contrast in night mode

- thumbnail clickable from comments
- Icons in comment nav bar need themeing
- Look into updating all newer java calls in the palette lib
- Comment nav bar
- Short scores
- Push notification not using same slider
- exoplayer keeping alive
- Pull to refresh on a sub starts from the cards rather than the sub forehead
- The counts at the top of a sub flicker
- Popup memus rounded
- Mark as read on scroll
- Selftext thumbnail not clickable	
- Disable rounded corners for full width cards
- Long press to open post in new window
- Short scores for the chip
- hide read doesnt dismiss the current video
	

## TODO

### Comments
	- Comment search + new design

### Cards
	- Autoplay for cards
	- Swipe actions need rounded corners

### Posts 
	- Update post adapter to use the UI mode
	- Optimise the post adapter
	- Hook up and test alt post types

### Bugs
	- Nav bar not fully hiding when scrolling
	- Volume indicator broken on inline gifs
	- Search in settings has a bugged toolbar

### Known issues
	- Dividers arent shown inbetween comments in the comment search bottomsheet
	- Missing favicons

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
	- Delete SelftextCardView
	- Remove LegacyCustomImageView
	- Delete slideimagewrapper
	- Revisit how missing thumbnails are generated

### Small issues
	- Remove any references to the old save logo