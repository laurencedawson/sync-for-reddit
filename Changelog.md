## Links

- [TODO](https://todo.syncforreddit.com)
- [Changelog](https://todo.syncforreddit.com/Changelog)
- [Beta discussion](https://todo.syncforreddit.com/discussion)


-----

# Sync v22.3.13

## Tablet
- The account picker is now much smaller
- Added tabbed comments!
- Settings is now dual pane on tablets

## Changes
- Increased the brightness of the primary text color in night mode
- Selftext previews now once again mark as visited
- Twitter previews now mark as read
- Settings are no longer locked to portrait
- Added search back in as a drawer item
- Disabled the comment open transition by default (default feels snappier)
- Huge refactoring to the Main/Casual activity
	- I don't think I've broken any navigation but please let me know...
- Pressing posts / messaging in the right section and scrolling to top will now show the restore snackbar
- Reverted the new message icon back to +
- The ripple in settings search is now the same as elsewhere in settingsx

### Fixes
- Fixed a crash when setting a sub thumbnail
- Fixed a crash when setting flair
- Fixed a list restore state issue

## Internal
- 

-----

# Sync v22.3.8

## Changes
- Added support for inline selftext image
- Added a new dark mode option "Dark overlay"
	- Decrease the screen brightness by 60% when in dark mode
	- Useful for bedtime browsing and not destroying your retinas
- Removed spaces in-between image flairs

### Fixes
- Fixed an issue where inline image previews couldn't be disabled
- Fixed an issue with posts not loading at the end of a list
- Fixed an issue causing the posts list to occasionally keep inertia when infinite scrolling
- Added another potential fix to help with the posts list crashing
- Fixed an old reference to the saved icon in the quick actions
- Fixed a video playback issue (would start in the background)

## Internal
- 

-----

# Sync v22.3.7

## Changes
- Secondary text is now a little lighter in dark mode
- OP icon has been updated & OP now highlights again
- All comment icons are now filled in
- Added a return to top FAB in the bottom nav subreddit picker
- Moved "open in new window" above fav in the subreddit menu
- Voting chip colors are a little darker now
- Voting chip now has a min width
- Added … to selftext previews
- Updated the search settings to use the new themeing
- Preferences now use the themed ripple
- Added an option to disable emotes
- Added an option to disable animated image comments

### Fixes
- The "push" preference has been updated to use the new switch style
- Fixed an issue where selftext images might fail to load on peek
- Fixed an issue where selftext images were not clickable
- Spoilers no longer autoplay (duhh)
- Fixed a few incorrect context crashes
- Fixed a crash when starting with biometrics enabled
- Added a potential fix for posts list crash
- Fixed displaying short scores in slides
- The current sub is now highlighted again in the subreddit picker / drawer
- Fixed an issue where the subreddit icon would used a cached value
- Fixed a rendering issue with tables in comments

## Internal
- Removed all traces of the old "accent color"
- Updated save to be the same everywhere

-----

# Sync v22.3.6

## Changes

- Fixed an issue with missing scores on compact views
- Added a little 👑 icon whenever ljdawson is shown
- Replaced username highlighting with icons
- Updated the style of the bottom loading bar (color + position)
- Popup menus now have rounded corners
- Messaging has been renamed to "inbox"
- Added "Inbox" and "Subs" to the quick actions (disabled by default)
- Long pressing the quick actions FAB will now perform the first selected action again
- Pinned post icons now show with the link color
- Added the option to move the image before title back for slides
- Changed the load / share icons in monet theme section
- Added a dropdown label next to the subreddit flair chip

### Fixes
- Fixed an issue that would cause the expanded toolbar to lose its position when changing between posts and messages
- Fixed an animation related crash
- Fixed an issue with a space showing on posts after inputting text...
- Mark as read on scroll has been added back in
- Fixed a crash when drawing a recycled animated emote
- Fixed an issue where the comment nav bar wouldn't show with no comments
- Fixed an issue where text was not visible in dark mode when selecting text
- Fixed an issue where domains were not showing for compact views
- Fixed an issue where clicking the hide button on a post kept the video playing

## Internal
- Unified all "post comments" into a single ViewHolder (comments in a profile or sub)
- Disabled "supportsPredictiveItemAnimations" in LinearLayoutManager to fix a longstanding issue

-----

# Sync v22.3.3

## Changes
- Added all view types back in (apart from swipe)
- Added AMOLED mode (Settings > Dark mode > AMOLED)
- Expanded the view options for slides (give it a try)
- Added an option to disable subreddit icons
- Added random to the default chips
- Reduced the alpha of a selected comment overdraw
- The search icon is no longer shown in the app bar
- Compact and smaller cards now have rounded thumbnails
- List is now even more compact
- Added extra padding to the bottom of the comments list when viewing a single comment
- The expanded toolbar is a little ^smaller
- Message style has been changed for nested messages
- When the FAB is configured to use "more actions" it now shows the sync icon

## Fixes
- Fixed a critical issue where text links were not clickable
- Fixed an issue with spoilers not rendering
- Fixed an issue with the subreddit showing in comments
- Full width images no longer have rounded corners
- Increased the left margin when no icon is shown in the toolbar


-----


# Sync v22.3.1

## Changes
- The version code now uses day of month too
- Removed the expand icon in the small toolbar
- Clickable inline links are no longer colored (domain & username)
- Attempting to change view now displays a message
- Voting + comment chip is now the same size as the post description
- Extra padding adding to the drawer FAB
- Inline link spans no longer use the link color
- Reset the key for showing labels in the bottom navigation

## Fixes
- Fixed the link underline issue
- Fixed a bug that would cause posts to display under the bottom nav (when autohide was disabled)
- Fixed a crash when leaving the app too quickly
- Fixed a crash when loading bottomsheets
- Fixed a crash when opening messaging
- Fixed a crash when re-arranging favs
- Fixed an issue causing search recents to have the wrong popup menu
- Fixed an issue where the old swipe to hide would conflict with the new post actions
- Fixed a crash when applying a tag
- Fixed a crash when starting the app
- Fixed a crash when generating a monet palette

## Updates
- com.google.android.material:material to 1.6.0-alpha03
- com.google.android.exoplayer:exoplayer-core to 2.17.0


-----


# Sync v22.1

## New

- A new Monet based themeing engine
	- When following the system color Sync will automatically update the colors if the system changes
- Added themed icon support for A13
- Swapped to a completely new image manager (bye bye IO Exception)
- Overhauled the settings with Monet theming
- Slides have been redesigned from the ground up (should be faster!)
- Slides now have subreddit icons
- Slides now have Twitter previews
- Added customisable swipe actions for posts
- Autoplaying videos have been completely rewritten to be much faster and smoother when scrolling
- You can now filter a subreddit by post flair from the expanded toolbar
- Slide site previews now have a fav icon
- You can now search from the subreddit bottom sheet
- Added "Click back to open the left drawer" back in
- Snackbars will once again show dark in dark mode
- Comments will now autoload top level "more"

## Changes

- Expanded the comments nav bar to include reply and collapse all (parity with v19)
- The number of awards shown is now capped to 3
- Card radius has been increased to match MD3
- Quick actions have been renamed More actions
- Reduced the number of default actions
- Removed presets from the settings
- Switched to the old drawer style (but with an option to increase open region)
- Updated the default title sizes for slides
- Disabled the chat icon in the sidebar
- Disabled search from the sidebar
- Disabled submit from the sidebar
- The save icon now matches reddit.com
- i.redd.it and v.redd.it domains are shown again in descriptions
- The selftest border is now only an option for slides
- Increased the size and changed the position of the image seekbar
- Zero width chars are now removed from selftest
- Colourful quotes are now disabled by default
- Deepzoom now has a default of 200dpi
- Sticky posts now feature an icon instead of changing the title color
- Preferences are now locked to portrait
- The search bottomsheet is now for searching posts
- The archived/np/locked banner now scrolls again

## Fixes

- Fixed the image upload / gallery select / edit functionality (submit and commenting)
- Fixed an issue with the drawer collapsing / expanding sections slowly

## Closed

- https://github.com/laurencedawson/sync-for-reddit/issues/732
- https://github.com/laurencedawson/sync-for-reddit/issues/729

## Notes

- 

## Internal

- Now targeting Android 12 (and testing on A13)
- Updated Exoplayer to v2.16.1
- All images are now handled by Picasso
- Updated WorkManager to v2.7.1
- Removed MultiDex
- Removed GSON
- Removed ConsentManager
- Removed jcenter references
- Removed androidx.ads:ads-identifier
- Removed all unused assets
- Removed firebase analytics
- Removed firebase messaging
- Removed com.reddit:indicator-fast-scroll
- Removed sectionedrecyclerviewadapter
- Removed gif-drawable
- Removed androidx.palette:palette