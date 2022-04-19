## Links

- [TODO](https://todo.syncforreddit.com)
- [Changelog](https://todo.syncforreddit.com/Changelog)

-----

# Sync v22.4.20

## New
- Added the A-Z picker back in as an option for the subreddit picker
- Added the option to "follow" users
- Added "mark as read" to post swipe options
- Post + Comment FABs can now be set to not autohide
- Added the option to disable recording top visited subreddits locally
- The URL preview shown on slides + cards now matches the same size as the post description
- Imgur galleries now show as inline image previews (sadly with a static image until we can figure something better)
- Selecting text in the editor and then clicking quote will now insert the selected text quoted
- Long pressing the comment reply FAB will now show more options

## Changes
- You can now select expanded toolbar AND disable autohiding
- Added a bottomsheet for the join subreddit chip
- Added a new style to the "watch subreddit" bottomsheet
- The splash screen on pre-Android 10 is now dark
- Contextual chips are now forced on if you have autohide toolbar disabled
- Added image resolution + file size to the image details
- Sharing a post preview now includes the subreddit + icon and NSFW images are now longer red
- The share button is now always shown in the posts "more" bottomsheet
- Upped the char limit from 10k to 40k
- Toggling accounts now ignores logged out
- Large previews are now always fetched for posts (when logged out)

## Fixes
- Domains are now shown again for slides
- Fixed an issue with themes not automatically updating on Samsung devices
- The fix underscore bottomsheet is now only shown for non-reddit links
- Added another fix for the infamous posts showing behind other posts issue
- Fixed an issue when selecting u_profile links in the subreddit picker
- Fixed an issue where youtu.be links would show as image posts
- Fixed a padding issue for cards when autohide toolbar is disabled
- Fixed an issue where Twitter profile pictures would get the wrong background in AMOLED dark mode
- Albums now respect the full height preview option
- Fixed an onboarding crash

## Closed
- https://github.com/laurencedawson/sync-for-reddit/issues/940
- https://github.com/laurencedawson/sync-for-reddit/issues/974
- https://github.com/laurencedawson/sync-for-reddit/issues/1074
- https://github.com/laurencedawson/sync-for-reddit/issues/1000
- https://github.com/laurencedawson/sync-for-reddit/issues/964
- https://github.com/laurencedawson/sync-for-reddit/issues/1056
- https://github.com/laurencedawson/sync-for-reddit/issues/991
- https://github.com/laurencedawson/sync-for-reddit/issues/835
- https://github.com/laurencedawson/sync-for-reddit/issues/969
- https://github.com/laurencedawson/sync-for-reddit/issues/992
- https://github.com/laurencedawson/sync-for-reddit/issues/1057
- https://github.com/laurencedawson/sync-for-reddit/issues/826
- https://github.com/laurencedawson/sync-for-reddit/issues/414
- https://github.com/laurencedawson/sync-for-reddit/issues/302
- https://github.com/laurencedawson/sync-for-reddit/issues/1073

## Internal 
- Removed dev.kdrag0n:colorkt
- Switched from AppLovin to Admob due to poor in-app performance 

## Updates 
- androidx.biometric:biometric > 1.2.0-alpha04
-----

# Sync v22.4.16

## New
- Added link + comment karma & profile creation to the about popup
- Added an option to highlight comments that are from new accounts (on by default)

## Changes
- OP and Friends are now highlighted again
- [Searching within a subreddit search will now give the option to search within that subreddit again](https://www.reddit.com/r/redditsync/comments/u2az1e/path_to_v22_release/i4hpj4c/)
- Changed how deeplinks open in app from coldstart
- Subreddit shortcut links (long press sync icon) now always open in sync
- The correct splash screen is now shown when opening a shortcut
- Subreddit shortcuts now use the subreddit icon
- Purchases are no longer reset when going to the restore page
- Added the ability to manually reset purchases on the restore page

## Fixes
- Added a fix for posts appearing behind other posts (animation glitch)
- Ads now have a min height to fix misclick issues
- Ads are now fully disabled when an activity pauses
- Fixed an issue where ads could be shown when starting sync from a deeplink

## Closed
- https://github.com/laurencedawson/sync-for-reddit/issues/891
- https://github.com/laurencedawson/sync-for-reddit/issues/832
- https://github.com/laurencedawson/sync-for-reddit/issues/1018
- https://github.com/laurencedawson/sync-for-reddit/issues/1001

-----

# Sync v22.4.12

## Changes
- Updated the purchase checker to use an alt method if querying fails
- Updated the style of setting links

-----

# Sync v22.4.11

## New
- Added a new onboarding / setup experience
- Added a new splashscreen with animation
- Improved the startup time for free significantly
- Added "recents" to the comment page "more" bottomsheet
- Added deeplinked settings

## Changes
- Dark mode preferences now use radio buttons

## Fixes
- Fixed an alignment issue for the embedded twitter description
- Fixed an issue where resetting the theme management preferences wouldn't reset the intensity
- Fixed a crash when viewing inline videos
- Fixed a 404 when clicking licenses
- Fixed an issue where changing typeface / relative size would require an app restart
- Fixed a visual glitch where clicking on the header in settings could respond to a click
- Fixed a bug where the account profile picture wouldn't show on first load

## Internal
- 

## Updates
- 

## Closed
- https://github.com/laurencedawson/sync-for-reddit/issues/959
- https://github.com/laurencedawson/sync-for-reddit/issues/962
- https://github.com/laurencedawson/sync-for-reddit/issues/1041
- https://github.com/laurencedawson/sync-for-reddit/issues/1027
- https://github.com/laurencedawson/sync-for-reddit/issues/1021
- https://github.com/laurencedawson/sync-for-reddit/issues/782
- https://github.com/laurencedawson/sync-for-reddit/issues/772

-----

# Sync v22.4.5

### Fixes
- Fixed an issue causing Exoplayer to use more battery
- Reverted changes previously made to exoplayer

-----

# Sync v22.3.30

## New
- 

## Changes
- Switched video caching to use a db with okhttp

## Fixes
- Fixed a crash in the image viewer
- Added an additional check when creating a video cache (should fix the cache exception error)

## Internal
- 

## Updates
- 

## Closed
- https://github.com/laurencedawson/sync-for-reddit/issues/950
- https://github.com/laurencedawson/sync-for-reddit/issues/946
- 

-----

# Sync v22.3.28

## New
- The background of fullscreen images is now colorful (can be disabled under Settings > Images)

## Changes
- Swapped the position of actions + explore
- Added additional padding above the image viewer seek bar to prevent misclicks
- Inline video playback should now feel snappier and smoother
- Hide is now always available in the post more menu
- Removed the "double width comment spacer" option as it no longer did anything
- Certain inline selftext images are now replaced with links (if they have crazy height to width ratios...)

## Fixes
- Fixed a crash when restoring backups made in .24 (will require re-setting the color intensity)
- Post inline videos are now paused when peeking
- Added a description under Subreddit icons in the settings
- Renamed "Show subreddit thumbnails" in the slides settings page
- Fixed an issue where the video position wouldn't be continued when opening a video full screen
- Fixed an issue where the Discord style panel would draw behind the status bar
- Added a potential fix for the autoplay battery drain issue
- Fixed an issue where videos might flicker the first frame from a previous video
- Fixed an issue that when hitting enter to search /r/FrontPage was incorrectly searched
- Fixed an issue where reddit videos could no longer be shared directly from the share menu
- Fixed an issue where the right hand side of the discord panel could be incorrectly opened
- Fixed an issue where clicking back in the internal browser would exit before going back through pages
- Fixed an issue where chevrons in Subreddit Sort panel can not be tapped
- Fixed an issue where the slider under theme management might be styled incorrectly
- Fixed an issue where search results would get "stuck" in the drawer or bottomsheet
- Fixed a crash when long pressing on quick actions with no actions available...
- Fixed an issue where Random NSFW had incorrect casing in quick actions
- Fixed an issue where a video could keep potentially playing after being hidden
- Fixed an issue where search links in comments could potentially crash or not open correctly
- Fixed an issue where ampersands were not playing nice with search
- Fixed an issue with spoilers showing in selftext
- Fixed an issue with the ban activity now styling correctly
- Fixed an issue where code after a horizontal rule messed up
- Fixed an issue where adding links in the comments editor could trigger a password manager
- Fixed an issue where posts might get stuck half way when changing subs
- Fixed an issue with notifications not being removed when mark as read was clicked
- Fixed a data saving related cockup
- Fixed an issue where images would load fullscreen behind the status bar with no padding
- Fixed an issue where inline videos were reporting they had audio when they did not
- Fixed an issue where escaped underscores wouldn't be handled correctly
- Fixed an issue where the gesture nav toolbar would flicker when opening images

## Internal
- Switched over from Mopub to Applovin (EOL)

## Updates
- 

## Closed
- https://github.com/laurencedawson/sync-for-reddit/issues/814
- https://github.com/laurencedawson/sync-for-reddit/issues/821
- https://github.com/laurencedawson/sync-for-reddit/issues/911
- https://github.com/laurencedawson/sync-for-reddit/issues/918
- https://github.com/laurencedawson/sync-for-reddit/issues/912
- https://github.com/laurencedawson/sync-for-reddit/issues/907
- https://github.com/laurencedawson/sync-for-reddit/issues/906
- https://github.com/laurencedawson/sync-for-reddit/issues/904
- https://github.com/laurencedawson/sync-for-reddit/issues/902
- https://github.com/laurencedawson/sync-for-reddit/issues/903
- https://github.com/laurencedawson/sync-for-reddit/issues/900
- https://github.com/laurencedawson/sync-for-reddit/issues/898
- https://github.com/laurencedawson/sync-for-reddit/issues/882
- https://github.com/laurencedawson/sync-for-reddit/issues/881
- https://github.com/laurencedawson/sync-for-reddit/issues/893
- https://github.com/laurencedawson/sync-for-reddit/issues/837
- https://github.com/laurencedawson/sync-for-reddit/issues/892
- https://github.com/laurencedawson/sync-for-reddit/issues/889
- https://github.com/laurencedawson/sync-for-reddit/issues/878
- https://github.com/laurencedawson/sync-for-reddit/issues/815
- https://github.com/laurencedawson/sync-for-reddit/issues/838
- https://github.com/laurencedawson/sync-for-reddit/issues/841
- https://github.com/laurencedawson/sync-for-reddit/issues/921
- https://github.com/laurencedawson/sync-for-reddit/issues/896
- https://github.com/laurencedawson/sync-for-reddit/issues/798
- https://github.com/laurencedawson/sync-for-reddit/issues/843
- https://github.com/laurencedawson/sync-for-reddit/issues/879
- https://github.com/laurencedawson/sync-for-reddit/issues/888
- https://github.com/laurencedawson/sync-for-reddit/issues/507
- https://github.com/laurencedawson/sync-for-reddit/issues/636
- https://github.com/laurencedawson/sync-for-reddit/issues/662
- https://github.com/laurencedawson/sync-for-reddit/issues/646
- https://github.com/laurencedawson/sync-for-reddit/issues/527
- https://github.com/laurencedawson/sync-for-reddit/issues/648
- https://github.com/laurencedawson/sync-for-reddit/issues/545
- https://github.com/laurencedawson/sync-for-reddit/issues/534
- https://github.com/laurencedawson/sync-for-reddit/issues/588
- https://github.com/laurencedawson/sync-for-reddit/issues/589
- https://github.com/laurencedawson/sync-for-reddit/issues/621
- https://github.com/laurencedawson/sync-for-reddit/issues/631
- https://github.com/laurencedawson/sync-for-reddit/issues/645
- https://github.com/laurencedawson/sync-for-reddit/issues/620
- https://github.com/laurencedawson/sync-for-reddit/issues/607
- https://github.com/laurencedawson/sync-for-reddit/issues/599
- https://github.com/laurencedawson/sync-for-reddit/issues/634
- https://github.com/laurencedawson/sync-for-reddit/issues/747
- https://github.com/laurencedawson/sync-for-reddit/issues/717
- https://github.com/laurencedawson/sync-for-reddit/issues/684
- https://github.com/laurencedawson/sync-for-reddit/issues/874
- https://github.com/laurencedawson/sync-for-reddit/issues/587
- https://github.com/laurencedawson/sync-for-reddit/issues/853
- https://github.com/laurencedawson/sync-for-reddit/issues/807
- https://github.com/laurencedawson/sync-for-reddit/issues/859
- https://github.com/laurencedawson/sync-for-reddit/issues/786
- https://github.com/laurencedawson/sync-for-reddit/issues/746
- https://github.com/laurencedawson/sync-for-reddit/issues/745
- https://github.com/laurencedawson/sync-for-reddit/issues/776
- https://github.com/laurencedawson/sync-for-reddit/issues/728
- https://github.com/laurencedawson/sync-for-reddit/issues/719
- https://github.com/laurencedawson/sync-for-reddit/issues/682
- https://github.com/laurencedawson/sync-for-reddit/issues/615
- https://github.com/laurencedawson/sync-for-reddit/issues/813
- https://github.com/laurencedawson/sync-for-reddit/issues/718
- https://github.com/laurencedawson/sync-for-reddit/issues/926
- https://github.com/laurencedawson/sync-for-reddit/issues/642
- https://github.com/laurencedawson/sync-for-reddit/issues/927
- https://github.com/laurencedawson/sync-for-reddit/issues/630
- https://github.com/laurencedawson/sync-for-reddit/issues/930
- https://github.com/laurencedawson/sync-for-reddit/issues/849
- https://github.com/laurencedawson/sync-for-reddit/issues/778
- https://github.com/laurencedawson/sync-for-reddit/issues/934
- https://github.com/laurencedawson/sync-for-reddit/issues/886
- https://github.com/laurencedawson/sync-for-reddit/issues/737

-----

# Sync v22.3.24

## New
- Theme management in the settings has been expanded to include
	- A new base color picker
	- Option to refine a color using sliders
	- A color intensity slider
	- Option enable a more colorful dark / light theme
	- An experimental option to replace link colors with the monet complimentary color for greater contrast

## Changes
- Archived and locked posts now use filled in icons
- The system navigation bar style has been updated
- Added "highlight stickied posts" as an option under **experimental**
- Fixed height inline videos have been added to experimental as a setting (off by default)

## Fixes
- Fixed an issue where the height of cards wasn't being respected
- Fixed an issue where the subreddit woudn't be updated in the search button when searching from the drawer
- Fixed an issue where images couldn't be shared to sync

## Internal
- 

## Updates
- 

## Closed
- https://github.com/laurencedawson/sync-for-reddit/issues/866
- https://github.com/laurencedawson/sync-for-reddit/issues/883
- https://github.com/laurencedawson/sync-for-reddit/issues/875
- https://github.com/laurencedawson/sync-for-reddit/issues/866
- https://github.com/laurencedawson/sync-for-reddit/issues/867
- https://github.com/laurencedawson/sync-for-reddit/issues/865
- https://github.com/laurencedawson/sync-for-reddit/issues/887
- 

-----

# Sync v22.3.21 (day 1 patch)

## New
- Added an option to enable "sliding panel style drawer" in the settings (Settings > Experimental)
- "Actions" can now be added back into the bottom navigation (Settings > Experimental)
- Long pressing Posts will now take you to your default subreddit
- Long pressing Inbox will now bring up the compose screen

## Changes
- Increased the default size of the slide + card description + comment description
- When tapping a search box in landscape the fullscreen keyboard is no longer shown
- The "Dark overlay" option now shows its selected state in more actions
- Pinned posts now show as colored along with the pinned icon
- Tweaked the ripple behaviour when unselecting a comment
- Disabled the "extended drawer open region" setting by default
- Increased the size of the image viewer seek bar & added a little padding left and right
- Search is now shown in the toolbar if you have bottom nav disabled

## Fixes
- Removed the "Example" chip in the Inbox chipgroup
- Fixed a bug where recents were not scrollable

## Internal
- 

## Updates
- 

## Closed
- https://github.com/laurencedawson/sync-for-reddit/issues/791
- https://github.com/laurencedawson/sync-for-reddit/issues/820
- https://github.com/laurencedawson/sync-for-reddit/issues/740
- https://github.com/laurencedawson/sync-for-reddit/issues/785
- https://github.com/laurencedawson/sync-for-reddit/issues/822

-----

# Sync v22.3.19

## Foldable / Tablet
- Support for large foldable devices (e.g. Fold 3)
	- When the main display is closed, the navigation rail will automatically become a BottomNavigationBar
- Slide / card cropped previews are now larger when tablet mode is enabled
- Tabbed comments are now disabled by default
- Added an option to force sync to respect additional window insets
- Tabs are now shown all the time if tab mode is enabled
- Clicking back on an open comments page now closes that page

## New
- 

## Changes
- The comment actions bar is now tinted with monet theming
- Youtube shorts are now excluded from the in-app YouTube player (do not work...)
- Tapping the toolbar in settings will now scroll to top


## Fixes
- Fixed a bug where changing between folded / open would result in your current section being lost
- Fixed an issue where the bottom progress bar wouldn't show without bottom nav
- Fixed an issue where keyboard wouldn't hide after selecting a search result
- Fixed a few tabbed comments bugs
- Fixed a bug where tapping the toolbar would return to the top of posts and comments
- Fixed an issue where clicking a comments tab twice would cause it to close
- Fixed an issue where the comments reply fab would show on scroll even if disabled

## Internal
- 

## Updates
- 

## Closed
- https://github.com/laurencedawson/sync-for-reddit/issues/805
- https://github.com/laurencedawson/sync-for-reddit/issues/757
- https://github.com/laurencedawson/sync-for-reddit/issues/759
- https://github.com/laurencedawson/sync-for-reddit/issues/811
- https://github.com/laurencedawson/sync-for-reddit/issues/809
- https://github.com/laurencedawson/sync-for-reddit/issues/753
- https://github.com/laurencedawson/sync-for-reddit/issues/810
- https://github.com/laurencedawson/sync-for-reddit/issues/777

-----

# Sync v22.3.17

## New
- Added "Dark overlay" to the quick actions
- Enabled large toolbar animations
- Slides now respect the option "long press to open comments in the background"
- Added an option to disable the comments reply FAB
- Added a "load color" button to the theme settings page
- Cards now autoplay again (single column only for now)
- Added a new animation for the large post toolbar

## Changes
- Autoplay has been fixed for slides
- Updated the style of contextual chips
- The refresh action now scrolls to the top of the list quickly before refreshing
- The first slide now has rounded corners again
- The "Top growing" chip has been replaced with "Change view"
- Removed the palette icon from the theme settings page
- Removed the save icon from the theme settings page

## Fixes
- Fixed an issue with the subreddit description flickering
- Fixed an issue with screen regions being blank when bottom nav hide was disabled
- Fixed an issue where the toolbar was autohiding when it shouldn't
- Fixed mis-coloring of comment navigation bar icons

## Internal
- You can now preview where autoplay starts (Setting > Developer)

## Updates
- 

## Closed
- https://github.com/laurencedawson/sync-for-reddit/issues/760

-----

# Sync v22.3.16

## New
- Long pressing "explore" will now open the explore sheet with search focussed (bottom nav + rail nav)
- Comment search has been hooked back up and has had a fresh lick of MD3 paint
- Added ripple effects to comments on click
- Added back in the moderator section
- Added an option for incognito keyboard (Settings > Security)

## Changes
- Removed the "focus on open" option from the explore menu
- Removed contextual chips from profile about / subreddit about
- Renamed Subs to Explore in the quick actions

### Fixes
- Fixed an issue where the text in a URL view was incorrectly highlighted
- Fixed a crash when tagging a user
- Fixed a crash when restoring tabbed comments

-----

# Sync v22.3.15

## New
- Search and subs have been unified into "Explore"
- Added icons for archived and locked posts
- Added the experimental option to open chrome custom tabs incognito

## Changes
- Increased the number of "top posts" to 25
- Increased the clickable region to activate the search box at the top of the subreddits picker
- Removed "search" as an item from the drawer as this can now be access from the existing search

### Fixes
- 

## Internal
- 

## Updates
- Exoplayer v2.17.1

## Closed
- https://github.com/laurencedawson/sync-for-reddit/issues/143
- https://github.com/laurencedawson/sync-for-reddit/issues/242
- https://github.com/laurencedawson/sync-for-reddit/issues/275
- https://github.com/laurencedawson/sync-for-reddit/issues/323
- https://github.com/laurencedawson/sync-for-reddit/issues/726
- https://github.com/laurencedawson/sync-for-reddit/issues/725
- https://github.com/laurencedawson/sync-for-reddit/issues/748
- https://github.com/laurencedawson/sync-for-reddit/issues/721
- https://github.com/laurencedawson/sync-for-reddit/issues/713
- https://github.com/laurencedawson/sync-for-reddit/issues/705
- https://github.com/laurencedawson/sync-for-reddit/issues/694
- https://github.com/laurencedawson/sync-for-reddit/issues/678
- https://github.com/laurencedawson/sync-for-reddit/issues/637
- https://github.com/laurencedawson/sync-for-reddit/issues/647
- https://github.com/laurencedawson/sync-for-reddit/issues/652
- https://github.com/laurencedawson/sync-for-reddit/issues/653
- https://github.com/laurencedawson/sync-for-reddit/issues/640

-----

# Sync v22.3.14

## Tablet
- Added support for a new tablet mode with side navigation rail
- Added support for dual pane in portrait & landscape
- Added tabbed comments!
- The account picker is now much smaller
- Settings now respect the dual pane mode

## Changes
- Added "contextual chips" back in as an option for the "more actions" bottomsheet
- *If the expanded toolbar is disabled, contextual chips are now always shown*
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
- The ripple in settings search is now the same as elsewhere in settings
- Renamed sections of messaging in the drawer to match the bottom navigation
- Removed redd.it link shortening

### Fixes
- Fixed a crash when setting a sub thumbnail
- Fixed a crash when setting flair
- Fixed a list restore state issue

## Internal
- 

## Closed
- https://github.com/laurencedawson/sync-for-reddit/issues/374
- https://github.com/laurencedawson/sync-for-reddit/issues/385
- https://github.com/laurencedawson/sync-for-reddit/issues/629
- https://github.com/laurencedawson/sync-for-reddit/issues/731
- https://github.com/laurencedawson/sync-for-reddit/issues/541

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