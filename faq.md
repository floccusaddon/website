---
layout: page
title: Frequently asked questions
description: "Find out more about how floccus does its magic."
---

# Which browsers are supported by floccus?
Currently floccus supports Chromium, Google Chrome, Mozilla Firefox, Opera, Brave, Vivaldi and Microsoft Edge.

# How can I access my bookmarks on my Android phone?
A Floccus Android app is available in an open beta [from the Downloads page](/download)

The only mobile browser to support extensions that interact with bookmarks is currently the free Kiwi browser.

# Does floccus support bookmarks tags in Firefox?
Unfortunately not, Mozilla has not yet added an API for interacting with native tags. However, floccus will not touch your tags.

# How are brower-internal URLs treated?
Browser-internal URLs like `chrome://` URLs are currently ignored and left alone. They may be supported in the future.

# How are non-HTTP URLs treated?
Since Nextcloud Bookmarks currently only supports HTTP links, URLs with any other schemes are ignored and left alone, when syncing via Nextcloud Bookmarks.
When syncing via WebDAV or Google Drive, `http(s):`, `ftp:, data: and `javascript:` bookmarks are supported.

# Does floccus track usage data at all?
No. Floccus does not track you in any way. The only network traffic initiated by floccus is syncing your bookmarks to the server of your choosing. That's it.

# How does floccus treat my cloud credentials?
As Floccus uses OAuth to connect to your Google Drive, it doesn't know and doesn't record your Google password. Instead, floccus stores an authentication token which can only be used to create new files and change the files created with the same token in your Google Drive. Not even floccus can access any other data stored in your Google services.

For Nextcloud you have the option to use your normal account password, or create a dedicated app token that you can revoke at any time.

For WebDAV, only a normal password can be used.

Floccus only stores the data you provide in your browser and doesn't send them anywhere. The aforementioned access credentials are thus as secure as your browser, by default. If even that is not enough for you, you can encrypt your credentials entered into floccus with a passphrase that you will have to enter on every browser start.

# I am currently using a different tool to sync my browser data. Can I use this with floccus?
No, any other sync tool affecting your browser bookmarks will lead to duplication and possibly corrupt data. Please disable any active browser syncing tool before using floccus.

# Some of my topmost folders are missing in one of my browsers. How can I avoid this?
Browsers usually do not allow you to create items in the toplevel root folder (/), that space is reserved for special folders like Mobile bookmarks, Bookmarks bar, Other bookmarks. Any attempts by floccus to create items inside the root folder (whether in Kiwi or on any other Browser) will fail. The intention is that the built-in Sync mechanism of the browser vendor or some other native browser process will create and manage these folders, so it's by design that extensions are not able to write to it.

If you are missing some toplevel folders on a browser, try setting a different local folder to sync to in the floccus settings. E.g. instead of syncing to the absolute root folder, sync to a folder one level deeper, like Bookmarks Bar on Desktop or Mobile Bookmarks on mobile.
