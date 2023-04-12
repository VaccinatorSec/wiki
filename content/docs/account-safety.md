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
This article serves as a quick reference guide of what to watch out for, and current methods attackers uses in order to compromise other user's account.

This is a brief document, it does not cover every possible attack vector, but it should cover the general gist of common things to watch out for.

You can visit the main article for each attack method to learn more about it.

## Key guidelines
These are not concrete guidelines, but they generally serve as a way to quickly discern if something is unsound:

### Too good to be true
If something is too good to be true, it probably is; The obvious one, if someone made a claim that seems too good to be true, they might not have clean intentions, as there is no such thing as a free lunch after all.

### Evaluate calmly
If you encounter a message which seems time sensitive and urgent, you should give yourself a moment of pause and evaluate it logically. It's a well known trick that such emotions is a good way to get humans to drop their guard and do things in a panic rush.

### Do not trust verified bots
Do not trust messages sent by a bot simply because it bears a verified tick; an attacker could have compromised the bot to deliver that message, or leverage any messaging feature like a DM greeting functionality.

### Watch out for impersonator
Do not believe it if any user or any bot that claims to communicate on behalf of Discord. Discord only communicates via the official "discord" account. Official discord accounts will also bear the "System" badge.
==todo screenshot of official thread==

## Consequences
Falling for one of these attacks can have drastic consequences.

The attacker can gain access to your account, which allow them to use your account to spam invites, or spread phishing over guilds and friend list. Your account may be banned or kicked from guilds, unfriended or blocked from others, or at worst case be banned and deleted from discord entirely.

This may also impact you financially, as the attacker might also attempt to spend your linked credit card to purchase nitro(which is sold on the black market) if any are present.

## Remediation
What to do if you have fallen for one of these attacks? as topic of remediation is complicated and have different steps depending on which attack vector was used, you should check out [Remediation Guide](./) for the full guide.

## Summary of methods
Below listed a summary of methods that an attacker might attempt to use in order to compromise someone's account.

The list here mainly applies to Discord, but some like phishing might be applicable to other spaces.

### Phishing
Main article: [Phishing](./threats/phishing)

Phishing is a type of attack where an attacker tricks users into giving sensitive credentials like usernames and passwords. Attackers can achieve this by impersonating another trusted website in order to trick the users into sending their credentials.

Most commonly found in the form of websites that claim to give you free nitro, sometimes they will use compromised users to leverage their friend's trust and spread their scam. You should question your friend if they happen to be spreading this kind of content.

When entering your password, pay attention to the URL bar on the browser, make sure it's `discord.com`, otherwise you risk sending your password to an attacker impersonating as Discord.

Here are some other signs to watch out for in relation to phishing:

#### Empty address
If the URL bar is blank/empty with no text as in "" or displayed as "about:blank", that means it's likely it's not actually on the site you expect it to be, but instead you are on a webpage controlled by an attacker.
==TODO Images for empty address==

#### Fake window
If the login window is a "popup" has the expected URL, try dragging the popup out of the current window, so that nothing else is behind the window, except your desktop wallpaper.
If you cannot do that, it's likely that's not a real browser window, but some cleaver trickery on the website, giving the illusion of a pop-up window with faked URL, this popup is also controlled by the attacker. Also see: [Browser in the Browser](./threats/phishing#Fake popup (Browser in the Browser))
==TODO images for popup==

### Malware
Main article: [TODO]()
Some attackers may instead attempt to trick users into downloading malware, when executed it will infect your system with virus, and it might send your discord token, browser cookies, browser passwords and so on to the attacker.
If someone asks you to download something, you decline and ignore, block them if they are relentless.

Attacker often employs a story of some sorts to trick and convince users, like "a student in game dev who need some play tester for their games", do not fall for their schemes, just politely decline it and move on.

Attackers might also use compromised accounts to leverage friend's trust and spread their malware, if your friend asks you to do so, consider validating checking if their account was hacked and is controlled by an attacker instead.

Sometimes they may take on appearances of things that are too good to be true, such as "download this for free nitro".

### Bogus verifications
Main article: [TODO]()
This section covers bogus ways of verification that serves as a pretext to get the user to do something which might compromise their own account.

#### QR Code
There's no QR based verification bot, if a bot is asking you to scan a QR code, it's probably trying to gain access to your account.

If you pay attention, the mobile Discord app will warn you that scanning and authorizing the QR code allows others to access your account, so do not scan it, do not click authorize.
==TODO mobile screenshots==

#### Bookmarklet
If a bot or website claims you need to add a bookmark and click it after visiting `discord.com` to verify, do not follow through. Doing so will allow the bookmarklet to execute code which grants the attacker access to your account.

### Developer tools
Main article: [TODO]()
Developer tools are a powerful console intended for use by developers, which can be accessed by pressing `Ctrl+Shift+I`. However, it contains numerous hazards that attackers could leverage to compromise the security of your account.

#### Malicious code execution
In the developer tools, there's a "console" tab which shows the console's logger and also allows JavaScript code to be run.

You should not copy and paste code from untrusted sources, as running code in the console could grant the attacker access to your account.

If someone is claiming you should run it with pretext, such as "verifying yourself" or "gain free nitro" or any of the things that are suspicious, you should avoid following along.

#### Leaking secrets
In the developer tools, there's a "network" tab which shows network request made by the JavaScript. The request might include secrets which an attacker could use in order to access your account, you should avoid opening it during a screenshot, recording, or screen sharing session.

You should avoid sharing the output of "Copy" option or "Save all as HAR with content" option, as both of them might include secrets that attackers can use to access your account.