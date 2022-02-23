Sync v22.1
-----

## New

- Added themed icon support for A13
- Swapped to a completely new image manager (bye bye IO Exception)
- Overhauled the settings with Monet theming
- A new Monet based themeing engine
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
- 

## Fixes

- Fixed the image upload / gallery select / edit functionality (submit and commenting)
- Fixed an issue with the drawer collapsing / expanding sections slowly

## Closed

- https://github.com/laurencedawson/sync-for-reddit/issues/732
- https://github.com/laurencedawson/sync-for-reddit/issues/729

## Notes

- 

## Internal

- Now targeting Android 12
- Updated Exoplayer to v2.16.1
- Swapped out Glide to Picasso	
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