---
date: '2026-11-04T19:49:54+03:00'
draft: true
title: 'first pipeline workflow?'
---

So I have a blog now. Didn't plan to, but here we are.

It started with a stupid command. The kind that can wipe a whole Linux system if you let it. Naturally, I pasted it to see what would happen.

That same night I found GitHub Pages, and I started wondering what I could actually do with it. Then I remembered that one of my mutuals on Twitter has his own blog, so I went digging to figure out how he built it. That led me to static site generators. I found a theme I liked on GitHub, built with Hugo.

And that's where it stopped being simple. Installing an app with `sudo snap install` is like walking. You never stop and wonder how you’re able to walk. Then Linux asks me for my password, and it hit me exactly like suddenly being conscious of walking. WHAT? I never set a password. I tried everything I could possibly remember. And yeah turns out WSL needed its own password. One I’d set once and completely forgotten. So I had to go into WSL as root from CMD and reset it. I think somewhere out there is a dude with 9 years of system administration experience getting ragebaited reading this. Cmon, I mean, shit happens right?

I installed Hugo. Finally. The theme I chose is called PaperMod, and I made sure to follow every setup instruction carefully. Then suddenly an error with `.Language.Direction` stopped everything. Turned out PaperMod needs version 0.158 or higher, but the Hugo package manager shipped an old one (0.154). So I had to remove the apt version and download the current one straight from GitHub as a `.deb`.  After some fighting, it finally built. The site ran locally. My first real win.

Now I had to do all the configuration using YAML files. It’s easy. Or so I thought. This was my first time dealing with YAML, the format and the syntax and the indentation.
