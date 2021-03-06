---
layout: default
title: Blog 2 SP21
date: '2021-03-05 16:30:00 -0700'
categories: blog update
published: true
---
<h1>Setting Up RTX Voice on a GTX Graphics Card</h1>
<p>I recently watched a YouTube video where someone was showcasing the software "RTX Voice" which was made by the tech company Nvidia. This software is able use an Nvidia RTX line of graphics card to remove background noise from your microphone. From what I saw the software looked like it worked really well, even blocking out the sound of a leaf blower. But because this software could only be used with an RTX graphics card, I was not able to take advantage of the software because I had a lower generation GTX graphics card.</p>

<p>Upon further research, there actually was a way to get RTX software working on a GTX graphics card. The first step is to run the RTX Voice installer so that the necessary folder and files are created. This is what should pop-up on the installer. <img src="https://i.imgur.com/pj9j6Or.png" width="540" height="460"> <br> Close the installer and navigate to the folder C:\Temp\NVRTXVoice in Windows Explorer. This is where the installer left the file that needs to be edited.</p>

<p>Located within the NVRTXVoice folder is another folder called NvAFX, and in that folder is a file called RTXVoice.nvi. <img src="https://i.imgur.com/sQZSOcg.png" width="640" height="200"> <br> Open this file using a text editing application and use ctrl-f to find this snippet of code. <img src="https://i.imgur.com/ug5WVqM.png" width="640" height="200"> <br> Delete this entire section and save & close the file. The final step is running the installer again, but this time from the folder itself, located in C:\Temp\NVRTXVoice\setup.exe. The installation should run without any issue and now you can use RTX Voice on a GTX graphics card.</p>