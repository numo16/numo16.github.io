---
layout: post
title: "Progress..."
date: 2010-10-25 21:39
comments: true
categories:  [Game Dev, Imagine Cup, Dev Ops]
---

Between classes, work, and figuring out everything for Imagine Cup 2011, I’ve been busy as hell.  Next week is my last week for both my Game Scripting and Data Structures and Algorithms class, which both take up a considerable amount of my available free time.  At work I’ve been wrapping up a market share study and implementing a few long awaited features for one of our main apps.  So, after those two, that has left me a few hours to deliberate over which theme to pick for Imagine Cup, figure out team members, and figure out the direction and concept of the game.  Between Zander and myself, with a nice random idea from Jarrod, I think we’ve nailed down exactly what we want to do for the competition.  Zander has decided he definitely wants in on this, so it is up to me at this point to decide if I’ll be able to spare the time to make this work, which I have pretty much decided that I will. In the meantime, I’ve decided to setup the project environment, complete with subversion repos, integration and build server, wiki, issue tracker, and a bunch of other things.  <!-- more -->Everything is setup and hosted on my server like so:

Subversion: [Collabnet Subversion Edge](http://www.open.collab.net/products/subversion/)
OK, so this setup is pretty awesome.  CSVN is a simple installable package, sporting a subversion server and a nice web management interface.  It can integrate with a few bug trackers and has nice connectivity with Visual Studio, thanks to their Ankh SVN plugin.  The best part, it’s free!

CI and Build Server: [Jetbrains TeamCity](http://www.jetbrains.com/teamcity/)
TeamCity is a pretty awesome setup.  It’s a free continuous integration and build server that will automatically build my projects whenever a new version is committed to the main repo.  This also has a great web management interface, allowing me to monitor builds, setup build scripts for projects, and also integrates with a few well known issue trackers.

Wiki, Issue Tracker, etc…: [TikiWiki](http://info.tiki.org/tiki-index.php)
I needed somewhere to have a central collaboration area, to keep all of our ideas and the project documented.  I thought about using media wiki at first, but after my first initial experience with dealing with that mess, I decided to seek out better alternatives.  TikiWiki seemed to fit the bill with its wiki, forum, issue tracker, and a bunch of other features I won’t end up using.  It’s pretty awesome.  The only problem I can foresee with it for this project currently, is that CSVN and TeamCity do not integrate with the issue tracker in TikiWiki, which means I may have to setup Bugzilla or something later.

Setting up the environment like this is a new thing to me, but after reading through several topics on [StackOverflow](http://stackoverflow.com/), it seemed like a good idea to setup the environment like this just to make everything a bit easier and a more automated, streamlined process.  I’m still working out the kinks, so time will tell if all of this will be a help or hindrance.  Next item on the docket, a better backup system…