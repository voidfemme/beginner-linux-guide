# [Linux Survival Guide](title)
---
## [Table of Contents](contents)
- [The Desktop](#the-desktop)
- [File Browser](#file-browser)
- [System Update](#system-update)
- [The Launch Menu](#launch-menu)
- [System Preferences](#preferences)
- [Downloading Software](#downloading-software)
- [sudo (root priviledge)](#sudo)
- [File Structure and Permissions](#file-structure-and-permissions)
- [Conclusion](#conclusion)
- [Further Reading & Learning](#further-reading)
---
## [First notes](first-notes)

First, right-click is the bottom right region of the trackpad. I may be able to
change this if it feels annoying to you. I prefer a two-finger right click, just
let me know if you'd like it changed.

## [The Desktop](the-desktop)
### [Bottom Left Panel](bottom-left-panel)
The desktop functions almost identically to Windows 10. If you put a file on the
desktop, it stores the file in /home/|[your username]/Desktop

On the bottom Left, you have the Linux Mint logo, which will open a menu, very
similar to the menu on Windows. From left to right:
- Toggle desktop (hides/shows all windows on the desktop)
- Firefox
- Terminal Emulator
- File browser

### [The Launch Menu](launch-menu)
The Launch Menu can be opened by clicking the Linux Mint logo in the bottom left
side of the screen. You can find all of your installed apps, as well as any
preferences you might want to check out. There is so much in there, so have a
look around and try to figure out what might be in there that can help you.

### [Bottom Right Panel](bottom-right-panel)
On the bottom right, from right to left, you have:
- Bell: opens your desktop notifications
- Sheild: System Update (make sure to check this regularly, Linux doesn't
  auto-update unless you explicitly enable that)
- The rest are pretty self-explanatory: Wifi status, battery status, volume,
  date and time.

You can right-click on any items of the bottom panel to rearrange, remove, or
access the bottom panel settings. You can even set the bar to whichever edge of
the screen you prefer: bottom, top, or either side. There are also different
kinds of widgets you can add, and it can be fun to check those out.

## [File Browser](file-browser)
Pretty much works the same as windows, but the more you use Linux, the more
familiar you'll get with it. The file browser can actually be replaced by any
other file browser application! But I suggest you try to get used to Linux
before getting too deep into changing stuff like that.

## [System Update](system-update)
Okay, so the system update screen (Sheild on the bottom right-hand corner) is
very important. If you want automatic updates, click the sheild to open system
update. Then go to Edit, then Preferences, then Automation.

## [Preferences](preferences)
First, you will notice that the preferences aren't all in one single location.
There are several different preferences application for each aspect of your
desktop and system. 

NOTE: sound can be really finnicky on Linux. When you are here and messing
around with it, let's make sure your sound is working as it should and exactly
how you want.

## [Downloading new applications](downloading-software)
If you need a new application, do not download something directly from the
internet. (there are exceptions to this, but you can learn those later) Instead,
open your Launch Menu, and type, "Software Manager" you can look for
applications that do what you want there. I am familiar with a lot of different
Linux apps, so if you're having trouble finding what you need, you can always
text me to ask for a recommendation. Otherwise, I suggest you experiment!

## ["sudo" - With Great Power Comes Great Responsibility](sudo)
Ok, so this one is a little bit more technical, but it's really important for
you to know. Sometimes if you google search for help or troubleshooting, you
will find people directing you to open the Terminal, and type commands. If the
first word of the command that you see is "sudo", **be very careful!** If you use
"sudo" without knowing what the command means, **you could accidentally break your
system!**

This is because "sudo" gives you root permission, with root permission, you can
delete, change, or move any system file, which could be disastrous, unless you
know what you are doing is safe. I'd just suggest avoiding any commands
involving "sudo" until you are more comfortable with linux.

**Keep in mind, that you will need to use the terminal at some point. Don't be
afraid of it! Just respect the power that the command line gives you.**

## [File Structure and Permissions](file-structure-and-permissions)
### [File Structure](file-structure)
Understanding your file structure is important, because it will let you know
where you can place your files, and where you may not. When you are logged in,
you have permission to modify every file in your home directory. A directory is
like a home address, and like Windows, the file structure is like a tree. Your
home directory's "address" is at /home/[your username]

in that address, the very first "/" symbol represents the address of the "root"
directory. In it you will find these files:
- /bin
- /boot
- /home
- /etc
- /usr

...among several more. I'll put a little bit of info about these later on. for
now, just know that all the files besides your home directory (/home/[your username]) are
off-limits.

### [Permissions](permissions)

"Permissions" refer to _which owner_ is allowed to perform _which actions_. There are
three important actions:
- Read
- Write
- Execute

There are three different types of ownership:
- User
	- If you created the file, or if it exists within /home/[your username], then you
	  are the owner.
	- If the file exists in any other root directory, then the owner is
	  "root". "root" is the same as the "system administrator"
- Group
	- A "group" is a set of users. If you have multiple user accounts on
	  your laptop, you can make a "group" by clicking on the Linux Mint logo
	  at the bottom left, then System, then Users and Groups. A group can
	  both regular users and root.
- Other
	- This basically means anyone else.

## [Conclusion](conclusion)
If you have any other questions, let me know, and I'll gladly add them to this
file! I'll download the file onto your computer, but I'll store this on my
Github repository so that you can see it and any changes I've made to it for you
at any time. Here's the online version:
https://github.com/voidfemme/beginner-linux-guide/edit/main/linux_survival_guide.md
