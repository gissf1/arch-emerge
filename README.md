arch-emerge
===========

In short, this is a pacman wrapper/frontend to emulate Gentoo's "emerge"
package management tool on ArchLinux systems.

Originally based on "pacsync" from https://gitlab.com/isd/pacsync Copyright (c) 2012, Ian Denhardt <ian@zenhack.net> and released under the ISC License.

A few paths combined to create this concept:

- I am a long-time Gentoo user, and I love how Gentoo's "emerge" package management tool provides a simple idempotent viewpoint on system packages. This perspective makes upgrades and migrations quite simple.

- I choose to run ArchLinux on my laptops for ease of maintenance, and I
had to perform a complex upgrade situation, so I was looking for a tool to more easily manage packages and remove unneeded dependencies on Arch, similar to how I handle it on Gentoo.  This led to me finding pacsync.

- Upon looking at the code for Ian's "pacsync", I was amazed at how simply it did exactly what I wanted.  In attempting to install it via the AUR package, I was surprised to discover that it conflicted with another 'pacsync' binary.  Upon investigating, I discovered that this name was already used by the pacman tool that syncs the repositories, which is obvisouly necessary for a properly functioning ArchLinux system.

- I prefer to use Gentoo's Emerge command line syntax, but I don't want to run any kind of hybrid system with multiple package managers, nor do I want to run a source-based distribution on my laptops.

Since ArchLinux's pacman package already contains a "pacsync" binary, Ian's pacsync concept is quite similar to how Gentoo's Emerge manages packages, and I prefer standardizing on Gentoo's emerge command anyhow, I decided to extend this project, rename it to 'emerge', and use it to wrap pacman with an emerge-like interface.

I have retained the original source license (ISC) on this project since it is quite flexible and retaining the original license likely simplifies any legal questions on code use elsewhere.  I will retain copyright and ownership of my contributions, but still allow for use under the original license so others can have the option to freely use it or contribute as I have.
