---
layout: post
title: "Sync with iTunes While You Sleep"
date: 2012-01-03 13:55
comments: true
categories:
---
Wi-Fi syncing in iOS 5 is great when you have iPhone docks everywhere and rarely connect your iPhone to your Mac. iOS 5 almost removes the need to sync at all, but iCloud is missing one feature: it doesn't sync downloaded podcasts.

This hack is great for daily syncing of your downloaded podcasts, played status, and listening progress. It will also back up your iOS devices, so I suppose that's good too!

## 1. Save this AppleScript to a file.
{% gist 1283363 %}

## 2. Set up a cron job to run the AppleScript.
I used [CronniX](http://code.google.com/p/cronnix/) to set up the cron job to run the command `osascript /path/to/file.scpt` every day at 7:00 AM.

![CronniX Screen Shot](/images/cronnix.png) 

## 3. Done.
That's it! Now all of your iOS devices will sync automatically each day as long as they're connected to Wi-Fi.

*New year's resolution to write at least one blog post in 2012 complete. See you next year.*