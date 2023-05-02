# LTMEAT - Easy tutorial taken from https://git.nebulaproxy.dev/Chloe/LTMeat
## what is it? 
LTmeat is an exploit basically takes advantage of Chrome's vulnerability in their process management, extension management, and internal URLs. LTmeat works by essentially giving an extension (the thread or worker of it, specifically), too much to do, and it freezes (or hangs). 
That's the most basic explanation of it. [Find out more](https://ltmeat.bypassi.com/)

## Steps
1. Open a tab in the Chrome browser. Find a page belonging to the extension you want to disable. `chrome://extensions`, `chrome://extensions-internals`, and `chrome://process-internals` are all good places to find your extension's ID (a 32-character lowercase string). 
    * **TIP:** For some filters like Securly, the block screen is already an extension page.
2. Copy your extension ID, and navigate to `chrome-extension://YOUR-EXTENSION-ID-HERE/manifest.json`
3. Bookmark the extension page (bookmark A) if you wish. Then, bookmark `chrome://kill (B)` and `chrome://hang` (C).
4. While on the extension page (A), click the `chrome://kill bookmark` (B). The page should crash. You should already have the next step prepared.
5. Instantly start spamming `chrome://hang` (bookmark C) and use ctrl+R to reload the page while spamming. 
    * **You should have reloaded within one or two seconds of killing the page!**
6. Okay, what now? 
    * If the extension page (bookmark A) no longer loads or becomes unresponsive, that means LTMEAT worked! You can close your tabs and the extension will essentially be fried. 





## Questions and Answers
Firstly, please, please make sure you did the instructions properly. 


Q - Nothing loads.
A - If nothing loads, then you probably reloaded too late. Restart your computer to revert back to normal.

Q - Why does extension page A become unresponsive? 
A - Because it shares the same memory process with the first tab.

Q - Do I have to do this every time i restart my Chromebook? 
A - Yes, [Read more: How does LTMEAT work?](https://ltmeat.bypassi.com/)

Q - I have more questions, where do I go? 
A - [Nebula Discord Server](https://discord.gg/unblocker) | [TitaniumNetwork Discord Server](https://discord.gg/unblock)
