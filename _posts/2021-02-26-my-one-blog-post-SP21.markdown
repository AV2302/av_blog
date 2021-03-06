---
layout: default
title: Blog 1 SP21
date: '2021-02-26 16:30:00 -0700'
categories: blog update
published: true
---
<h1>Setting Up Wake-On-LAN for Windows 10</h1>
<p>On my PC, I run a media server using an app called Plex so that I can watch all of my local media, such as movies and shows, on any smart-tv in my house that supports Plex. I don't have my PC running at all times because I don't use the Plex server often, so when I do want to watch something, for example downstairs, I would have to go up and turn on my PC to have the server running. Due to my own laziness I decided to research how I could remotely power on my PC.</p>

<p>Through my research, I discovered that there is a feature that Windows has had for a long time apparently called "Wake-On-LAN". This feature allows a computer, that is in a low power state, to wait for a "magic packet" that is sent by your router to the PC. Once that packet is received, the PC will power on. I wasn't aware just how many steps it took to enable this feature. <br> <img src="https://i.imgur.com/AKSFCgi.jpeg" width="650" height="300"> <br> I thought just by enabling Wake on LAN in my bios that it would just work, but there was more to it than that.</p>

<p>Beside just enabling Wake on LAN in your bios, you must also enable in Windows. This is done by going to Device Manager, then finding your network adapter, going to its properties, and enabling  Wake on Magic Packet. <br> <img src="https://i.imgur.com/AKBQ405.png" width="400" height="480"> <br> Once you've done that, you have to go into Power Options, Choose what the power button does, and disable Turn On Fast Startup. After these steps have been taken, you can now use a Wake-On-LAN app on your Smartphone to signal your router to send the magic packet, powering on your PC </p>