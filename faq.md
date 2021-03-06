---
layout: page
title: Frequently asked questions
description: "Find out more about how floccus does its magic."
---

# Which browsers are supported by floccus?
Currently floccus supports Chromium, Google Chrome, Mozilla Firefox, Opera, Brave, Vivaldi and Microsoft Edge.

# How can I access my bookmarks on my phone?
The only mobile browser to support extensions that interact with bookmarks is currently the free Kiwi browser.

Alternatively, if you're syncing via Nextcloud bookmarks, you may use one of its companion mobile apps.

# Does floccus support bookmarks tags in Firefox?
Unfortunately not, Mozilla has not yet added an API for interacting with native tags. However, floccus will not touch your tags.

# Does floccus track usage data at all?
No. Floccus does not track you in any way. The only network traffic initiated by floccus is syncing your bookmarks to the server of your choosing. That's it.

# How does floccus treat my cloud credentials?
As Floccus uses OAuth to connect to your Google Drive, it doesn't know and doesn't record your Google password. Instead, floccus stores an authentication token which can only be used to create new files and change the files created with the same token in your Google Drive. Not even floccus can access any other data stored in your Google services.

For Nextcloud you have the option to use your normal account password, or create a dedicated app token that you can revoke at any time.

For WebDAV, only a normal password can be used.

Floccus only stores the data you provide in your browser and doesn't send them anywhere. The aforementioned access credentials are thus as secure as your browser, by default. If even that is not enough for you, you can encrypt your credentials entered into floccus with a passphrase that you will have to enter on every browser start.

# I am currently using a different tool to sync my browser data. Can I use this with floccus?
No, any other sync tool affecting your browser bookmarks will lead to duplication and possibly corrupt data. Please disable any active browser syncing tool before using floccus.
