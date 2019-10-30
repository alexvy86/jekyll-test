---
layout: post
title:  "Hello world 2!"
date:   2019-10-29 23:42:13 -0500
categories: jekyll update
---
I’ve been using [Microsoft OneDrive’s Personal Vault][personal-vault] feature for sensitive documents for a while now and overall I’m pretty happy with it. But recently I noticed that after I unlocked the folder in my computer, double-clicking a PDF file opened up Acrobat Reader DC (my default PDF reader) but I got the following error:

![There was an error opening this document. Access denied](/assets/acrobat-error.png)

After some googling I found that this seems to be an issue with Acrobat Reader’s [Protected Mode][acrobat-protected-mode] feature. The intention behind it is good (sandboxing the PDFs that you open, so they can’t wreak havoc indiscriminately in the computer), but in this particular case it was hindering me.

Since I only put PDFs in my Personal Vault after I’ve “vetted” them, and I’m pretty careful with what I open in general, I decided it was fine for me to disable Protected Mode by going to `Edit -> Preferences -> Security (Enhanced)​` and unchecking `Enable Protected Mode at startup`:

![Disabling enhanced security](/assets/acrobat-protected-mode.png)

And voilà! PDFs from my Personal Vault now open correctly when I double click them.

[personal-vault]: https://onedrive.live.com/about/personal-vault/
[acrobat-protected-mode]: https://helpx.adobe.com/reader/using/protected-mode-windows.html
