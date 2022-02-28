## Links

- [TODO](https://todo.syncforreddit.com)
- [Changelog](https://todo.syncforreddit.com/changelog)
- [Beta discussion](https://todo.syncforreddit.com/discussion)

## Work in progress

	- Alpha release

## TODO

### Comments
	- Comment search + new design

### Cards
	- Hook up the new inline video player for cards	
	- Add the new pinned posts header

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