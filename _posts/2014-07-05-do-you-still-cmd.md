---
layout: post
title: Do you still CMD?
cover: 'assets/images/cover2.jpg'
date: '2014-07-05T15:55:00.001+05:30'
subclass: 'post tag-test tag-content'
categories: 'ram'
tags:
    funread
    newonshelf
    nonfiction
    thriller
    historicalfiction
    philosophy
    tragedy
    adventure
    goodreads
    mystery
    poems
    shortstories
    childrensfiction
    feminism
    movie
    preorder
    war
logo: 'assets/images/ghost.png'
---

Hey there, long time no see! Yeah right, you and I both have a full time job that only gives us time enough to watch an episode of *Man vs Wild*! Alright, I'll get to the point.

So the question was, how many of us use the good old *Command Prompt* these days? How many of us have switched to _PowerShell_? How many of us still type in short commands in the _Run_ window to launch applications? Honestly, I still open the Run prompt and type in `powerpnt`, `chrome`, `iexplore`, `appwiz.cpl`, `gpedit.msc`, etc. I don't know why, but I like to launch stuff this way. My brother still stares at me when I launch Notepad by saying `notepad`. Of course, I do admit, using `Run` is kinda old-school in this age of voice control.

Deviating a little bit, I remember one of my friends posting a comment on Facebook, when I updated my status about my progress with learning PowerShell, stating, "Oh, the new Command Prompt in Windows 7?" That's a major misconception when it comes to PowerShell. I don't blame him, for he isn't into the Windows domain&mdash;he's more of a (non-Microsoft) Cloud Backup guy, but what he said is a general misconception among people&mdash;they think PowerShell is the same as Command Prompt. Fact: it isn't. We'll discuss how, some other time.

Coming back to using the Command Prompt, I ran a verbal mini-survey, on a bunch of my buddies from different domains, about their usage of the Command Prompt. Turns out, in the current environment, they "are very comfortable with the use of `CMD`" I smiled. They added that they use it "to find the IP address"; one of them even added, "so cool, huh!" Indeed! I thought for a second, had they known that they could simply type in `ip address` in their Chrome address bar, it could give them their IP address, would it then mean that they wouldn't use the Command Prompt at all? I wouldn't know unless I tell them this alternate way of finding their IP address which would seem "cooler".

Anyway, so that's the outlook that common people have with the Command Prompt. There's this another interesting thing one of my friends said, "Don't you think it is like dumb to use the Command Prompt when you have your interface?" By that, she meant the Graphical User Interface. Well, I wouldn't call it dumb to use the Command Prompt when you have your GUI&mdash;a simple example, your IP address. Finding the IP address using GUI isn't a small task on Windows. This is how you do it: `Start\Control Panel\Network Connections\Local Area Connection\Properties\Internet Protocol (TCP/IP)\Properties`. Smart!

Some of us have another opinion about the Command Prompt, that "it is dull". Sure, agreed that it looks pretty dull with the black background and a grey foreground (no, it isn't white&mdash;try it for yourself). The interface is pretty dull and geeky, but hey, it comes in handy when you don't have to go all `Control Panel\bla-bla\bla-bla-bla\bla-bla-bla-bla...`!

And some think it is "showing off" when we use the run prompt and type in `control` when we need to go to the Control Panel or `appwiz.cpl` when we, say, wanna uninstall _Citrix Receiver_? "Convenience", that's the word. Personally, I'm very comfortable with the keyboard and have a pretty good typing speed (thanks to QWERTY everywhere), and I use _a lot_ of keyboard shortcuts. I love the keyboard and prefer using it instead of the touchpad to do a lot of stuff like this. Like say I wanna turn this part of the sentence to Consolas 10pt, font colour: 85% grey, opt not to check spelling or grammar, set the line spacing to single, set to "don't hyphenate", all I do is, press `Ctrl + Alt + C`! (Don't try that yet, or you might get the © symbol; you need to manually configure this one, once, in Word, before you can get the result).

And why am I writing this? Just to say that using the Command Prompt is an efficient thing to do when you need to get work done quickly, and its purpose is not to just check the IP address of your computer (and that there's an alternative to that too). The Command Prompt or even the Run prompt is a great thing to have, when you need to launch specific programs, or even shut down a remote computer. Seriously! I'll give you a short list of the cool things that you can do with the Command Prompt.

Before that, I'll narrate to you a situation that I got stuck in, one day. I had launched this Command Prompt window through Citrix _Web&nbsp;Interface_ once to get a list of all the members (recursive) in a security group in our organisation. After this, I wanted to launch a session of _Excel_ from the same server because the license had expired on my local machine. I re-launched the WI and thanks to some cookie crap in the current session of Internet Explorer (which I couldn't close because there was another process running in the background), that the WI said, "invalid session" or something. I tried launching another session of IE, but that didn't work either. Stuck? Nope! I switched to the Command Prompt Window, typed in `excel` and bingo!

Alright, as promised, here are some of the cool general-use commands that you can use from the Run prompt:

| Command                   | Function                                      |
| ------------------------- | ----------------------------------------------|
| `calc`                    | Launch the Calculator                         |
| `charmap`                 | View the Character Map                        |
| `chkdsk`                  | Launch the Check Disk Utility                 |
| `cmd`                     | Launch the Command Prompt                     |
| `control`                 | Go to the Control Panel                       |
| `timedate.cpl`            | Open the Date and Time Properties             |
| `cleanmgr`                | Launch the Disk Clean-up Utility              |
| `firefox`                 | Launch Mozilla Firefox                        |
| `fonts`                   | Open the Fonts Folder                         |
| `iexplore`                | Launch the Internet Explorer                  |
| `logoff`                  | Log out of Windows                            |
| `moviemk`                 | Launch the Movie Maker                        |
| `mspaint`                 | Launch Microsoft Paint                        |
| `control netconnections`  | Open Network Connections                      |
| `notepad`                 | Launch the Notepad                            |
| `osk`                     | Launch the On-Screen Keyboard                 |
| `perfmon`                 | Launch the Performance Monitor                |
| `control printers`        | Open Printers and Faxes (under Control Panel) |
| `mstsc`                   | Launch the Remote Desktop application         |
| `control schedtasks`      | Open Scheduled Tasks                          |
| `services.msc`            | Open Services                                 |
| `shutdown`                | Shut down the computer                        |
| `msinfo32`                | View the System Information                   |
| `taskmgr`                 | Launch the Task Manager                       |
| `explorer`                | Launch the Windows Explorer                   |
| `magnify`                 | Launch the Windows Magnifier                  |
| `wmplayer`                | Launch the Windows Media Player               |
| `write`                   | Open WordPad                                  |

Oh, if you're wondering how `explorer` could come in handy when you already have it running, imagine that you got the message that "Windows Explorer has encountered a problem and needs to shut down"! No, don't panic! Just press `Ctrl + Shift + Esc` (`Ctrl + Alt + Delete` seems like a death command combination to some who've used the pre-XP versions of Windows. Both these combinations open the _Task Manager_) Oh, and trust me, nothing goes wrong by opening the Task Manager; unless you go to the _Processes_ tab and kill some unrelated-but-very-important process that brings down the whole system. Opening the Task Manager _doesn't kill the computer_, like some people think. If you're scared to use the key combination (when Explorer is still running), right click on the _Taskbar_ and select `Task Manager`.

Now, click on `Run New Task`. You'll now get the Run prompt; type in `explorer` and hit `Enter`. There, you have your beloved Windows Explorer in front of you&mdash;aww… look at those moist eyes on seeing the Taskbar again!

Would you use the Command Prompt now?

Cheers!
