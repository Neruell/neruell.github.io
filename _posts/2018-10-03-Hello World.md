---
layout: post
title:  "First Post - GoDaddy and Github Pages"
date:   2018-10-03 00:34:22 +0200
categories: blog-posts
---

# GoDaddy and Github Pages

I was recently doing some changes to a Webpage for a friend, [Institut-Apart.de](https://institut-apart.de).  

## History

Now long story short. This was an old page I created several years ago. This is a *static* webpage, which means, no server-side code. The only server-sided functionality was obviously the `mail()` function, to send E-mails. Long time ago I used a free host [https://www.000webhost.com/](https://www.000webhost.com/), which allowed for a decent version of php and for the `mail()` functionality. Also an important thing to notice, it had **no branding** for hosting! For a free webhost, it is quite rare to find. It went good, with no issues for several years.  

Recently a friend wanted me to do some changes to the website, just *minor* things, nothing big. So I did, and of course reuploaded the needed files.  

## Current events  

Since some time, the webhost did change the pricing and billing options, and of course included some branding for a free plan. So after the changing files, they included the branding, a **no-go** for me. So went ahead to search for other webhosts. Unfortunately was not lucky to find anything which is  

*reliable  
*free
*php support for `mail()`  
*no branding  

That's why searching for a static webpage hosting made more sense, rather than just to search for a webhost with multiple <unnecessary> options. Found some interesting and funny solutions, like hosting with **Dropbox**, or **GDrive** using an *old* Account. But **Github** also supported hosting, and since I was using it for storing the webpage anyway, so I decided to try it out, also since it allows for *custom domain*, and built-in *ssl support*. Nothing really hard to setup. <Surprisingly>, it was pretty painless and easy, nothing extraordinary.  

Of course I had to go to **GoDaddy** to setup the <A Name> with the new IP Addresses. Also a lot of Tutorials, Videos, ~Documentation~ for it. All of them show the same thing. Just do this and that, easy! Did everything that I had to. Waited several minutes for the changes to take place. Went to GitHub Repo's Settings Page. <Your website is ready!>. Cool, want to add *ssl support*? Well just wait 24 hours! OK, no problem. The Website is reachable and is working as intended. 

## 24 Hours later  

Well, not really exactly 24 hours, but almost. Went to the settings page, and I see the message <Your domain is not pointing towards the GitHub Page URL>. Clicked on it, and the website still works fine. No isuees. Weird... Went to GoDaddy, all settings seem fine. Was changing stuff everywhere and sometimes, the GitHub Page said that the Webpage is ready, but the actual Webpage just showed an error message: <This website is temporarily unavailable, please try again later>. Some time later, it will be the other way round. Webpage works fine, no errors, but the GitHub Page literally says the same error as before, custom domain is not pointed towards the GitHub Server...  

Now this is **always** the time for every developer, where they waste tons of time for no reason. I tried almost everything  

*changing settings on GitHub  
*changing settting on GoDaddy  
*deleting the Repo, recreating it  
*changing A Names  
*changing Repo Name  
*...  

I guess pretty much every option was tried, except for the literally stupid ones. So after **a lot of time** wasting on stuff, why not try those. Let's make a redirect on GoDaddy for the same webpage for an infinite loop. Said and done. Trying to open the page, of course results in an error, for *too many redirects*. Go back to GoDaddy to remove the setting for the Redirect. That results in a complete *wipe* of all your settings for that domain. Like a <Hard Reset>. Nothing to lose anyway, so said and done. Also had to reenable the **A Names**. Waited for the changes to take place. Went to GitHub, and **WHAT IS THAT**? Instant SSL Support, and no error anymore.  

## Conclusion  

It seems that the GoDaddy settings were either wrong, or were not saved correctly or something was really broken on their end, because although the old settings were removed, several times (changing the A Names), and it took a complete <reset> to wipe some internal settings. Afterwards it worked fine. No issues, and GitHub never showed anymore errors again and also allowed for SSL Support, so no *up to* 24 hour waiting.  

So if you have any similar issues with domain names on GoDaddy, just try to set/unset redirect, or to <reset> settings if possible.