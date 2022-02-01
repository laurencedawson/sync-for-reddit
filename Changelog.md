Sync v22.1
-----

## New

- Slides have been redesigned from the ground up (should be faster!)
- Slides now have subreddit icons
- Added customisable swipe actions for posts
- Autoplaying videos have been completely rewritten to be much faster and smoother when scrolling
- You can now filter a subreddit by post flair from the expanded toolbar

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

## Fixes

- 

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