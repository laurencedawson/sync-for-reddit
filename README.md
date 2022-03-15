## Links

- [TODO](https://todo.syncforreddit.com)
- [Changelog](https://todo.syncforreddit.com/Changelog)
- [Beta discussion](https://todo.syncforreddit.com/discussion)

## Work in progress

### Missing
- Adjust how bottom nav height is caluclated
- Comment search
- Mod tools

- quick action for dark overlay
- back in dual pane should close that comments view
- Add dropdown icon next to small toolbar again
- refresh should go to top of list first
- monet refine!!

- When bottom nav is disabled, move where the bottom progress bar is
- option to disable fab in comments
- Add rounded corners back to slides
- Inconsistent vote icons (posts v slides)
- Sidebar...
- Icons in comment nav bar need themeing
- Comment nav bar
- The counts at the top of a sub flicker
- Long press to open post in new window
- comment nav can get stuck when you tag someone
- Profile pics not aligned in comments
- Show currently picked sub in the picker	
- issue https://www.reddit.com/r/redditsync/comments/t671kf/bug_using_the_keyboard_while_viewing_posts_eg_to/hzgwq9g/?context=3	
- friend chip not working
- Potential jank when hiding extended toolbar
- Add more details to profile bottomsheet	
- Submit shows a legacy alertdialog
- FIX MOBPUB ADAPTER HELPER
- "Long press cards to open comments in the background doesn't seem to be working for the Slides view type"
- Growing chip

## TODO

### Cards
	- Autoplay for cards
	- Swipe actions need rounded corners

### Bugs
	- Nav bar not fully hiding when scrolling
	- Volume indicator broken on inline gifs
	- Scroll to top broken (in tablets)

### Missing
	- Swipe mode

### Known issues
	- Dividers arent shown inbetween comments in the comment search bottomsheet
	- Requires a restart to change text font / sizes
	- When a bottomsheet dialog is shown and the display is off, it doesn't theme

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
	- Old dialog when submitting + selecting images