---
layout: default
parent: Changelog
title: In-development
nav_order: 1
---

# In-development

----------

## Ultra
- 

## New
- Sort and more actions will appear as "top sheets" when accessed from the toolbar ([#1381](https://github.com/laurencedawson/sync-for-reddit/issues/1381)_
- Website previews, expanded links and image links have been added to selftext ([#1292](https://github.com/laurencedawson/sync-for-reddit/issues/1292))
- Added "copy code block" buttons after code blocks in comments / selftext
- Added a popup for Dev users to come join the Discord!
- Ehnanced autoplay. Grab higher quality autoplay videos with audio for Gfycat &amp; Redgifs ([#827](https://github.com/laurencedawson/sync-for-reddit/issues/827))

## Changes
- YouTube link handling is now off by default due to an update from YouTube breaking the player
- Added additional text when sharing images with titles directly
- Updated the settings reset icon
- Enabled "[fast fallback](https://old.reddit.com/r/RedditEng/comments/v1upr8/ipv6_support_on_android/)" for all requests. This should fix any IPv6 releated issues ([#1389](https://github.com/laurencedawson/sync-for-reddit/issues/1389))
- Long pressing spoilers now performs the click action instead ([#1131](https://github.com/laurencedawson/sync-for-reddit/issues/1131))
- User flairs are now restricted to 20 characters and can be tapped to reveal the full length ([#519](https://github.com/laurencedawson/sync-for-reddit/issues/519))
- Changed how multi-line code is rendered ([#1336](https://github.com/laurencedawson/sync-for-reddit/issues/1336))
- If translate is not available a toast is now displayed ([#1324](https://github.com/laurencedawson/sync-for-reddit/issues/1324))
- Swipe view selftext is now set as the primary text color
- Added a fallback loading method for Gfycat & Redgifs
- Gfycat & Redgifs now load HD variants on WiFi
- YouTube thumbnails are now loaded directly ([#1347](https://github.com/laurencedawson/sync-for-reddit/issues/1347))
- If media fails to download to a subfolder it will now automatically recreate the folder ([#1177](https://github.com/laurencedawson/sync-for-reddit/issues/1177))
- Youtube previews now use a higher quality version ((#1137)[https://github.com/laurencedawson/sync-for-reddit/issues/1137])
- Post previews are now generated for every sub by default
- Simplified enabling / disabling inbox replies ([#1369](https://github.com/laurencedawson/sync-for-reddit/issues/1369))
- 

## Fixes
- Fixed an issue with wiki links not being clickable ([#1405](https://github.com/laurencedawson/sync-for-reddit/issues/1405))
- Fixed an issue with wiki pages sharing the incorrect link ([#1411](https://github.com/laurencedawson/sync-for-reddit/issues/1411))
- Fixed an issue where the bottom nav region would persist when disabled ([#1425](https://github.com/laurencedawson/sync-for-reddit/issues/1425))
- Fixed an issue where "View mods" was missing from the About page ([#1422](https://github.com/laurencedawson/sync-for-reddit/issues/1422))
- Fixed an issue where icons were not shown behind swipe actions in tablet mode  ([#1415](https://github.com/laurencedawson/sync-for-reddit/issues/1415))
- Fixed an issue where copying post titles would append a zero-width space at the end ([#1413](https://github.com/laurencedawson/sync-for-reddit/issues/1413))
- Fixed a restore issue ([#1412](https://github.com/laurencedawson/sync-for-reddit/issues/1412))
- Fixed an issue where white lines could appear around images when using full-width mode ([#489](https://github.com/laurencedawson/sync-for-reddit/issues/489))
- Fixed an issue on Android 7 where the search box would appear overly rounded
- Fixed an issue where bottom navigation items were not long clickable on Android 7 ([#1305](https://github.com/laurencedawson/sync-for-reddit/issues/1305))
- Fixed an issue where drafts were not readable in night mode ([#1216](https://github.com/laurencedawson/sync-for-reddit/issues/1216))
- Fixed an issue where searching with # caused it to disregard the subreddit ([#1171](https://github.com/laurencedawson/sync-for-reddit/issues/1171))
- Fixed an issue where the more actions bottom sheet would remain up ([#1428](https://github.com/laurencedawson/sync-for-reddit/issues/1428))
- Fixed a crash when exiting the app
- Fixed a crash when opening the legacy drawer
- Fixed a crash when searching for a subreddit
- Fixed an issue where Gfycat links would not show as media previews ([#1329](https://github.com/laurencedawson/sync-for-reddit/issues/1329))
- Fixed status bar issues when in split screen ([#1270](https://github.com/laurencedawson/sync-for-reddit/issues/1270))
- Fixed an issue where text was not scrollable in swipe mode ([#1406](https://github.com/laurencedawson/sync-for-reddit/issues/1406))
- Fixed an issue where videos wouldn't resume in fullscreen from card mode ([#1223](https://github.com/laurencedawson/sync-for-reddit/issues/1223))
- Fixed an issue where "select text" wasn't scrollable ([#1120](https://github.com/laurencedawson/sync-for-reddit/issues/1120))
- Fixed a swipe issue when using the discord style drawwer ([#1431](https://github.com/laurencedawson/sync-for-reddit/issues/1431))
- Fixed an issue where multiple spaces in selftext / comments were combined to one ([#1264](https://github.com/laurencedawson/sync-for-reddit/issues/1264))
- Fixed an issue where long clickin a username would fail to open externally ([#1281](https://github.com/laurencedawson/sync-for-reddit/issues/1281))
- Fixed an issue where images that were webpages were not displaying the right error ([#1176](https://github.com/laurencedawson/sync-for-reddit/issues/1176))
- Fixed an issue where escaped spoiler tags were rendering as spoilers ([#1361](https://github.com/laurencedawson/sync-for-reddit/issues/1361))
- Fixed an issue where quotes couldn't be placed inside quotes ([#1361](https://github.com/laurencedawson/sync-for-reddit/issues/1361))
- Fixed an issue where super long selftext iamges would crash ([#1404](https://github.com/laurencedawson/sync-for-reddit/issues/1404))
- Fixed an issue where updating the subreddit search term would reset the sort ([#305](https://github.com/laurencedawson/sync-for-reddit/issues/305))
- Fixed an issue where the wrong subreddit in the drawer could be highlighted ([#1242](https://github.com/laurencedawson/sync-for-reddit/issues/1242))
- Fixed an issue where messages were checked at startup even when disabled ([#798](https://github.com/laurencedawson/sync-for-reddit/issues/798))
- Fixed an issue where website previews in selftext / comments were displayed incorrectly
- Fixed an issue where the about bottomsheet would popup again if links were long pressed
- Fixed an issue where award bottomsheets used the old style for buttons
- Fixed an issue where images were saved incorrectly in swipe mode ([#1410](https://github.com/laurencedawson/sync-for-reddit/issues/1410))
- Fixed an issue where the keyboard wouldn't adjust the text input area ([#1254](https://github.com/laurencedawson/sync-for-reddit/issues/1254))
- Fixed an issue with Twitter previews in slides using fullwidth
- Fixed an issue with full width slides when all buttons were disabled ((#1149)[https://github.com/laurencedawson/sync-for-reddit/issues/1149])
- Fixed an issue where text with a strikethough would randomly update ((#1299)[https://github.com/laurencedawson/sync-for-reddit/issues/1299])
- Fixed an issue with low quality thumbnails ([#1121](https://github.com/laurencedawson/sync-for-reddit/issues/1121))
- Fixed an issue with content filters ([#1316](https://github.com/laurencedawson/sync-for-reddit/issues/1316))
- Fixed a crash with strange reddit video posts ([#1084](https://github.com/laurencedawson/sync-for-reddit/issues/1084))
- Fixed an issue where videos would not autoplay when using a mouse wheel ([#1333](https://github.com/laurencedawson/sync-for-reddit/issues/1333))

## Internal
- Removed the legacy CustomIpv4Dns class. Gfycat IPv6 requests will now automatically "fast fallback" to v4
- Developer options can now be accessed by /r/redditsync mods in the settings
- Added a way to demo the Discord join BottomSheet in the developer options
- Removed the secret panel
- FCM token can now be viewed in the developer options

## Updates 
- com.squareup.okhttp3:okhttp > v5.0.0-alpha.8

([]())