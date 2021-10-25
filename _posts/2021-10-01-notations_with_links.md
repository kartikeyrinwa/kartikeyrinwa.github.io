---
layout: post
title: "LaTeX and links to definitions."
categories: general
author: David Martínez-Rubio
excerpt_separator: <!--more-->
comments: true
---

Recently, I have been playing around with an idea I had some time ago about defining commands in LaTeX for all the notations you use (which is considered good practice) with the extra twist that the command wraps the notation with a hyperlink so you can place a hypertarget at its definition. In this way, you can automatically generate (non-highlighted) links for all of your notations just by using your commands (or if you don't feel like using so many commands when writing, you can always do some substitutions afterwards).

---

In this way, people reading your documents can click on any relevant math in order to jump to the place in the document where it was defined. I plan to write a more detailed post about how to achieve this, but for the moment [here is a sample](https://arxiv.org/pdf/2109.03678.pdf) so you can see how the implemented idea looks like (actually that one jumps exactly to the definition, which is too low for most readers. My current local version works more nicely).  

---

This feature is really nice, but if you really want to enjoy it, you should learn how to jump back after clicking on a link, or you will find yourself annoyed and scrolling back all the time. For the time being, I provide here a small table with some PDF readers and the shortcuts that are used to jump back.

---
### Readers and jumping back

| Reader | How to go back |
|-------|--------|
| Zathura | Ctrl + o (like in vim) |
| Firefox | Alt + Left  |
| Chrome | No option for jumping back :/ |
| Adobe Acrobat Reader| Alt + Left  |
| Okular  | Shift + Alt + Left  |
| Evince | Alt + p | 
| Pdf Reader Pro | Press the `jump back` button |
| Xodo (Android or iOS)| Arrows appear |

<!--
| Reader | How to go back | How to follow a link | Notes |
|-------|--------|---------|---------|
| zathura | Ctrl + o (like in vim) | Double click or f+number | Shortcut can be customized |
| Firefox | Alt + Left | Single click | A nice box appears when the mouse pointer is over the link. The viewer is really pdfjs (can be installed in some other browsers, like Chrome/Chromium) |
| Chrome | No option of going back | Single click | One can install pdfjs extension (called PDF Viewer), which is what Firefox uses by default |
| Adobe Acrobat Reader: Alt + Left | Single click |
| Okular  | Shift + Alt + Left | Single click | Shortcut can be customized |
| Evince | Alt + p | Single click | |
| PDF Reader Pro | Press `Jump Back` button | Single Click | |
| Xodo (Android or iOS): Arrows appear | Single tap | |

-->
