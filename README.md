## Links

- [TODO](https://todo.syncforreddit.com)
- [Changelog](https://todo.syncforreddit.com/Changelog)

# Current

	- https://github.com/laurencedawson/sync-for-reddit/issues/744
	- https://github.com/laurencedawson/sync-for-reddit/issues/951

	- https://github.com/laurencedawson/sync-for-reddit/issues/940

	- https://github.com/laurencedawson/sync-for-reddit/issues/832

----------------------------

# Main before release

- Add "search subreddits" to the actions part of the explore tab. Clicking this would open the old subreddit search from v19

- Videos need to be rejigged from the floating implementation

- Rounded corners shouldn't show for cards

- Swipe mode

- Add view type to onboarding

- Add expanded links
  https://github.com/laurencedawson/sync-for-reddit/issues/767

- Multi column inline videos
  https://github.com/laurencedawson/sync-for-reddit/issues/789

- Monet overrides!


- Theme management automatic and manual buttons are not working correctly

----------------------------


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