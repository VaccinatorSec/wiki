---
title: "Account Safety Crash Course"
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
This article serves as a quick at a glance resource to provide information of what to watch out for and current methods attacker uses in order to compromise other's account.

This is a brief document, it might not cover every single vector of attack, but it should cover the general gist of the common things to watch out for.

You can visit the main article for each vector to learn more about them.

## Key guidelines
These are not concrete rules but in general they serve a guideline that allows you to quickly discern if something is unsound:

### Too good to be true
If it's too good to be true, it is too good to be true; The obvious one, if someone claims something that's too good to be true, they might not have pure intentions.

### Approach with calmness
If something is attempt to create a shock or panic or rush in the reader, ex: false accusations, they are probably just trying to get you to drop your guard, and do something you normally wouldn't out of panic.

If you encounter such content, you should give yourself a moment of pause and evaluate it logically, it's a well known trick that using creating such emotions is a good way to get humans to drop their guard and do things they otherwise might not have done under a calm mind.

### Verified bot has no trust worthiness 
Do not believe messages sent by bot simply on the virtue of it bearing a verified tick, an attacker could have compromised the bot to deliver that message

### Discord only communicates via official thread
Do not believe it if anyone or any bot claims to communicate on behalf of discord

## Summary of methods
Below listed summary of methods which attacker might attempt to use in order to compromise someone's account.

The list here is mainly specific to discord, but some like phishing might be applicable to other spaces.

### Phishing
Main article: [TODO]()

When entering your credentials, pay attention to the URL bar on the browser, make sure it's `discord.com`, otherwise you may be sending your credentials to an attacker impersonating as discord

Here's also some other things to watch out for related to phishing:

#### Empty address
If the URL bar is blank/empty with no text as in "", that means it's likely it's not actually on `discord.com` ==TODO Images for empty address==

#### Fake window
If the login window is a "popup" with the correct URL, try clicking the URL bar and see if it's editable, or if you can drag the popup, so that nothing else is behind the window, except your desktop
If you cannot do any of the things listed above, it's likely that's not a real popup window, but a fake window controlled by the attacker ==TODO images for popup==

### Malware
Main article: [TODO]()
Some attackers may instead attempt to trick users into downloading malware, when prompted simply "don't".

They often employ a story or sorts to trick convince users, like "a student in game dev who need some play tester for their games", do not fall for their schemes, just politely decline it and move on.

Sometimes they may take on appearances of "things that are too good to be true", like "download this for free nitro"

### Bogus verifications
Main article: [TODO]()
This section covers bogus ways of verification that serves as a pretense to get the user do something which might compromise their own account

#### QR Code
There's no QR based verification bot, if a bot is asking you to scan a QR code, it's probably trying to get access to your account.

If you actually paid attention, the mobile discord app will warn you about scanning it will let others access your account, so don't do that.

#### Bookmarklet
If a bot or website claims you need to add a bookmark and click it on `discord.com` to verify, don't. Doing so will allow the bookmarklet to send the credential(token) back to attacker's servers.

### Developer tools
Main article: [TODO]()
Developer tools is a powerful console meant for developers, which can be accessed by pressing `Ctrl+Shift+I`, but it's something that contains numerous hazards which attackers could leverage to compromise the security of your account.

#### Malicious code execution
In the developer tools, there's a "console" tab which shows the console's logger and also allows javascript code to be ran.

You should not copy and paste code from untrusted sources, as code ran in there have the capabilities to exfiltrate your credential(token) and send them off to attacker's servers.

If someone is claiming you should run it with pretense like "verifying yourself" or "gain free nitro" or any of the things that are suspicious, you should avoid it.

#### Leaking secrets
In the developer tools, there's a "network" tab which shows network request made by the javascript.

The request might include things like your credential(token), you should avoid opening it while in a recording or screen sharing session. You should also avoid sharing the results of "Copy" option or "Save all as HAR with content" option as both of them will include your credential(token), sharing this will grant attackers access to your account