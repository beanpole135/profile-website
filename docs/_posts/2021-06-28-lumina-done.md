---
title: "Finished with Lumina"
date: 2021-06-28T08:00:00-04:00
categories:
  - Development
  - Projects
tags:
  - Lumina
  - Qt
---

So I have officially handed over maintainership of the Lumina Desktop and all it's tools to [JT Pennington](https://github.com/q5sys) now.
It has been a long road. I started the project on my "insomnia" nights back in 2012, mainly because I was frustrated by the instability of the Linux-developed desktop environments on FreeBSD (since I was using PC-BSD as my main system at the time). It started as just a simple wrapper to startup Fluxbox and pre-setup some common configuration elements. Then I made a floating panel and task manager because the Fluxbox one was both ugly and did not behave properly on multi-monitor systems. Then a wallpaper system... then all the XDG standards support (`lumina-open`, startup application support, etc...). Then all the tools started being needed. A calculator. A text editor, an `xrandr` manager, a PDF viewer... things that were difficult to find/use on FreeBSD systems, even though Linux apps were available.
Before you knew it, Lumina had been merged into PC-BSD. That is when the bulk of the tools/development happened for Lumina, because I was now able to work on it full-time as part of my duties for the PC-BSD project. Then the name change from PC-BSD to TrueOS. While nothing changed on my end right away, this started shifting a lot of my responsibilities from Desktop-support over to general non-graphical system utilities (`sysadm` in particular) as part of my day job, so Lumina started getting less attention. Give it another year or so, and I was now put in charge of developing the new "TrueView" project at iXsystems (eventually to be renamed to "TrueCommand" before it's initial release). By this point my work-time "priorities" were TrueView, TrueOS, and then any time left was for Lumina. 

Then out of left-field came the TrueOS "refocus", which basically cut the desktop side of the project out and we were given about a month to migrate Lumina and other desktop tools elsewhere. I started Project Trident with JT as a place to store/maintain all these desktop tools and frameworks initially, and then we gradually started moving them to more permanent homes.

While the Project Trident history is it's own story, the effect on the Lumina project was that the little time left to it was now pulled away into PT. After a couple years we got PT running smoothly with little/no maintenance required, but by that point there had been so many other life changes and pop-up projects that I just could not realistically dedicate time to picking up Lumina and doing major development on it again. The Qt5 -> Qt6 conversion was going to be significant (if it even works right on Qt6 - they seemed to go out of their way to remove a lot of the desktop-oriented functionality from the library), and the most of my maintenance of Qt apps was showing me a trend of breakage and/or removal of common functionality within the library.


## Where am I going from here?
I have been working on several other projects - one of them for almost 3 years - which I am getting ready to release. The main commonality among these tools is that they are all written in a programming language called "go"... and I am loving it. For long-term support of a utility, a static-build system is the way to do it, since upstream changes (looking at you Qt) will no longer break existing versions of tools.

Keep an eye out. My love of tabletop RPG's is finally meshing with my programming background....
