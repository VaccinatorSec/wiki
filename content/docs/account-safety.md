---
title: "Account Safety Awareness Crash Course"
description: "A breif guide to account safety awareness on discord."
lead: ""
date: 2023-03-29T22:10:23-04:00
draft: false
images: []
menu:
  docs:
    parent: ""
weight: 999
toc: true
---
## Overview
This article serves as a quick reference guide, to provide information of what to watch out for and current methods attackers uses in order to compromise others' account.

This is a brief document, it does not cover every possible attack vector, it should cover the general gist of common things to watch out for.

You can visit the main article for each attack method to learn more about it.

## Key guidelines
These are not concrete guidelines, but they generally serve as a way to quickly discern if something is unsound:

### Too good to be true
If it's too good to be true, it probably is; The obvious one, if someone claims something that's too good to be true, they might not have clean intentions.

### Approach with calmness

If you encounter such content, you should give yourself a moment of pause and evaluate it logically. It's a well known trick that such emotions is a good way to get humans to drop their guard and do things they otherwise might not have done under a calm mind.

### Verified bot has no trustworthiness 
Do not trust messages sent by a bot simply because it bears a verified tick; an attacker could have compromised the bot to deliver that message.

### Discord only communicates via official thread
Do not believe it if anyone or any bot that claims to communicate on behalf of Discord.

## Summary of methods
Below listed a summary of methods that an attacker might attempt to use in order to compromise someone's account.

The list here mainly applies to Discord, but some like phishing might be applicable to other spaces.

### Phishing
Main article: [Phishing](./threats/phishing)

When entering your password, pay attention to the URL bar on the browser, make sure it's `discord.com`, otherwise you risk sending your password to an attacker impersonating as Discord.

Here are some other signs to watch out for in relation to phishing:

#### Empty address
If the URL bar is blank/empty with no text as in "", that means it's likely it's not actually on the site you expect it to be, but instead you are on a webpage controlled by attacker, you should not enter your password here.
==TODO Images for empty address==

#### Fake window
If the login window is a "popup" has the expected URL, try dragging the popup out of the current window, so that nothing else is behind the window, except your desktop wallpaper.
If you cannot do that, it's likely that's not a real browser window, but an iframe on the website, giving the illusion of a pop up window with faked URL, you should not enter your password here.
==TODO images for popup==

### Malware
Main article: [TODO]()
Some attackers may instead attempt to trick users into downloading malware, when prompted you should decline and ignore, block them if they are relentless.

Attacker often employs a story of some sorts to trick and convince users, like "a student in game dev who need some play tester for their games", do not fall for their schemes, just politely decline it and move on.

Sometimes they may take on appearances of things that are too good to be true, such as "download this for free nitro".

### Bogus verifications
Main article: [TODO]()
This section covers bogus ways of verification that serves as a pretext to get the user to do something which might compromise their own account.

#### QR Code
There's no QR based verification bot, if a bot is asking you to scan a QR code, it's probably trying to gain access to your account.

If you pay attention, the mobile Discord app will warn you that scanning and authorizing the QR code allows others to access your account, so do not scan it, do not click authorize.
==TODO mobile screenshots==

#### Bookmarklet
If a bot or website claims you need to add a bookmark and click it after visiting `discord.com` to verify, do not follow through. Doing so will allow the bookmarklet to execute code which grants attacker access to your account.

### Developer tools
Main article: [TODO]()
Developer tools are a powerful console intended for use by developers, which can be accessed by pressing `Ctrl+Shift+I`. However, it contains numerous hazards that attackers could leverage to compromise the security of your account.

#### Malicious code execution
In the developer tools, there's a "console" tab which shows the console's logger and also allows JavaScript code to be run.

You should not copy and paste code from untrusted sources, as running code in the console could grant attacker access to your account.

If someone is claiming you should run it with pretext, such as "verifying yourself" or "gain free nitro" or any of the things that are suspicious, you should avoid following along.

#### Leaking secrets
In the developer tools, there's a "network" tab which shows network request made by the JavaScript. The request might include secrets which an attacker could use in order to access your account, you should avoid opening it during a screenshot, recording or screen sharing session.

You should avoid sharing the output of "Copy" option or "Save all as HAR with content" option as both of them might include secrets that attackers can use to access your account.