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
- Added a top secret new hidden panel...

## Changes
- Added additional text when sharing images with titles directly
- Updated the settings reset icon
- Enabled "[fast fallback](https://old.reddit.com/r/RedditEng/comments/v1upr8/ipv6_support_on_android/)" for all requests. This should fix any IPv6 releated issues ([#1389](https://github.com/laurencedawson/sync-for-reddit/issues/1389))

## Fixes
- Fixed an issue with wiki links not being clickable ([#1405](https://github.com/laurencedawson/sync-for-reddit/issues/1405))
- Fixed an issue with wiki pages sharing the incorrect link ([#1411](https://github.com/laurencedawson/sync-for-reddit/issues/1411))
- Fixed an issue where the bottom nav region would persist when disabled ([#1425](https://github.com/laurencedawson/sync-for-reddit/issues/1425))
- Fixed an issue where "View mods" was missing from the About page ([#1422](https://github.com/laurencedawson/sync-for-reddit/issues/1422))
- Fixed an issue where icons were not shown behind swipe actions in tablet mode  ([#1415](https://github.com/laurencedawson/sync-for-reddit/issues/1415))
- Fixed an issue where copying post titles would append a zero-width space at the end ([#1413](https://github.com/laurencedawson/sync-for-reddit/issues/1413))
- Fixed a restore issue ([#1422](https://github.com/laurencedawson/sync-for-reddit/issues/1422))

## Internal
- Removed the legacy CustomIpv4Dns class. Gfycat IPv6 requests will now automatically "fast fallback" to v4

## Updates 
- com.squareup.okhttp3:okhttp > v5.0.0-alpha.8


([#]())