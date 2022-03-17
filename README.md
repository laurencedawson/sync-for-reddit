## Links

- [TODO](https://todo.syncforreddit.com)
- [Changelog](https://todo.syncforreddit.com/Changelog)

## Work in progress

### Missing

- Growing chip
- option to disable fab in comments

- monet refine!!
- Autoplay for cards
- Need a clear way to show the default subreddit
- back in dual pane should close that comments view
- Add dropdown icon next to small toolbar again
- "use double width comment indents"
- Comment dividers
- When bottom nav is disabled, move where the bottom progress bar is
- Icons in comment nav bar need themeing
- Comment nav bar
- comment nav can get stuck when you tag someone

## TODO

### Pre-beta
	- Update ad network

### Bugs
	- Nav bar not fully hiding when scrolling
	- Volume indicator broken on inline gifs
	- Scroll to top broken (in tablets)

### Missing
	- Swipe mode

### Known issues
	- Requires a restart to change text font / sizes
	- When a bottomsheet dialog is shown and the display is off, it doesn't theme

### Refactoring
	- Check what is still using legacy activity
	- Go through and remove any calls to the old HTML to Spannable parser
	- Remove any references to ColorUtil.isColorDark (should just be using the palette now)
	- ColorUtils.setAlphaComponent
	- Delete custom positive button and negative button (use the new component)
	- Remove all final references to the old theme manager (StyleSingleton)
	- Look into changing the ripple drawable everywhere
	- Delete SelftextCardView
	- Remove LegacyCustomImageView
	- Delete slideimagewrapper
	- Revisit how missing thumbnails are generated
	- Refactor all GradientDrawable backgrounds
	- Look into updating all newer java calls in the palette lib