
---
layout: post
title:  "Installed!"
date:   2025-07-09 21:11:01 +0200
categories: projects
---

# LVM
It seems like LVM is completely unnecessary if the installation consists of only 2 partitions, of which only 1 is encrypted. 
Somehow I have assumed that LVM is necessary when using LUKS, which I now understand is not true. 
All my previous experience with manual partitioning in Linux have been dual boots with macOS, else I’ve just used automatic partitioning and checked the encryption box.

Anyhow, while looking into this encryption debacle I was hoping to run into as best practice, which I have not. The remains option is to ask our favorite word predictor: chatgpt!

ChatGPT gave me more than I asked for literally. 
If the LLM generated instructions worked I’ll post them.
(I basically asked for best practice when it comes to full disk encryption in Arch, but did it half in Swedish, half English so I’ll abstain from posting the slightly incoherent prompts).

In the end I went for a combination of [this guide from Wai Hon](https://whhone.com/posts/arch-linux-full-disk-encryption/), [the official guide](https://wiki.archlinux.org/title/Installation_guide) and ChatGPT.

# Attention to details
Being computer proficient, I thought installing Arch would be a breeze - but the encryption seemed to break everything all the time.
On the other hand - if I'd had a bit more attention to details, this would have been so much faster.

# Issues
The only problem now is that the keymap doesn't seem to load before decryption, which means a bot of hassle when typing passphrase, since it seems to load an English keymap.


To-do list:
- [ ] Make system load keymap before decyption
- [ ] Have a look at [Post-installation/General Recommendations](https://wiki.archlinux.org/title/General_recommendations)
	- [ ] Install GUI!
- [ ] Figure out audio setup in Arch
- [ ] Applications
	- [ ] Mixxx
	- [ ] Renoise
	- [ ] InkScape
	- [ ] GIMP
	- [ ] Audacity
	- [ ] Obsidian
