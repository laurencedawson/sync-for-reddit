## Links

- [TODO](https://todo.syncforreddit.com)
- [Changelog](https://todo.syncforreddit.com/Changelog)
- [Beta discussion](https://todo.syncforreddit.com/discussion)

## Work in progress

- Icons for user, OP, friend

- Add rounded corners back to slides
- inconsistent save icon
- Inconsistent vote icons (posts v slides)
- option to disable fab in comments
- Selftext thumbnail not clickable	

- add messaging and profile to actions
- add option to move position of image for slide
- Sidebar...
- Monet more contrast in night mode
- thumbnail clickable from comments
- Icons in comment nav bar need themeing
- Comment nav bar
- Short scores
- Push notification not using same slider
- exoplayer keeping alive
- The counts at the top of a sub flicker
- Mark as read on scroll
- Long press to open post in new window
- Short scores for the chip
- comment nav can get stuck when you tag someone
- Profile pics not aligned in comments
- Show currently picked sub in the picker	
- issue https://www.reddit.com/r/redditsync/comments/t671kf/bug_using_the_keyboard_while_viewing_posts_eg_to/hzgwq9g/?context=3	
- friend chip not working


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
	- Refactor all GradientDrawable backgrounds
	- Look into updating all newer java calls in the palette lib


### Small issues
	- Remove any references to the old save logo

### Bigger issues
	- Expand mod https://www.reddit.com/r/Android/comments/t6iz4l/sync_for_reddit_is_getting_a_complete_material/hzc6g0b/?context=3