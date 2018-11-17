---
layout: post
title:  My experience with Cryptocurrency mining
date:   2017-07-27 15:30:00
categories: Cryptocurrency Mining Blockchain Personal Review
tags: Cryptocurrency Mining Blockchain Personal Review
---

Today, I am going to write an article about my personal experience with cryptocurrency mining. If that sound crazy to you, well...it isn't. You can really earn money just by letting your computer/s switched on and connected to the Internet. The most important things in this business are video cards, not CPU or RAM.

**But why is that so?**...Well let me quote from a wiki:
> A CPU is an executive. A CPU is designed primarily to be an executive and make decisions, as directed by the software. For example, if you type a document and save it, it is the CPU's job to turn your document into the appropriate file type and direct the hard disk to write it as a file. CPU's are also highly capable of following instructions of the "if this, do that, otherwise do something else". A large bulk of the structures inside a CPU are concerned with making sure that the CPU is ready to deal with having to switch to a different task on a moment's notice when needed.

> A GPU is a laborer. A GPU is very different. Yes, a GPU can do math, and can also do "this" and "that" based on specific conditions. However, GPU's have been designed so they are very good at doing video processing, and less executive work. Video processing is a lot of repetitive work, since it is constantly being told to do the same thing to large groups of pixels on the screen. In order to make this run efficiency, video processors are far heavier on the ability to do repetitive work, than the ability to rapidly switch tasks.

Reading through it we will learn that GPU can do a lot of repetitive work comparing with CPU in less time, but it's not the best in this chapter. I am talking about ASIC (application-specific integrated circuit) Miner, which is an IC (integrated circuit) programmed for a particular use, here, mining. This might be the best choice because of the efficiency (electricity used vs coins mined).

I personally tested an Antminer S7 (mining bitcoin) which was pretty profitable at that time when I was doing the test: was producing ~10$/day, and the profit was ~7$/day. That sounds nice, but keep in mind that difficulty has raised and now the Antminer S7 is no longer profitable because now it's producing almost 4$/day (it's no longer profitable).

After this experience, I was pretty excited about mining crypto and tried to do also some tests with video cards, but with a different coin(Ethereum). I built 2 mining rigs with this specs each:

* Motherboard: Gigabyte 990FXA-UD3 R5
* CPU: AMD FX(tm)-4320 Quad-Core Processor
* RAM: 4GB Kingstone Fury
* HDD: SSD 120Gb Fury
* Video cards: 2* Radeon R9 Fury X 4GB HBM 4096-bit
* PSU: 2* ZALMAN ZM600-GSII 220V, with a homemade 2 PSU adapter

<img class="img-responsive image-center thumbnail" src="{{site.url}}/img/mining/pc_opened_2_gpus.jpg" alt="PC Open Case" />

I achieved almost 30Mh/s per video card, summing a total of ~120Mh/s, producing ~13$/day with a profit of ~9-10$/day. I admit that the PSUs are not used at all of their capacity, meaning that both rigs were consuming almost 1kW/h from the outlet. Also keep in mind that I mined in a pool, not solo, because of my low hashrate and bad luck :3

<img class="img-responsive image-center thumbnail" src="{{site.url}}/img/mining/2_pcs_mining.jpg" alt="2 PCs Mining Cryptocurrency" />

If you mine solo, it's not that important the high hashrate as the luck...Yes, you can have 500Mh/s and find a block in 2-3 days or 2-3 weeks. So, if you don't want to waste the hashpower, just join a pool. There are a lot out there: ethermine (1% fee with PPLNS payout scheme), ethpool (1%fee, paid after you solve a block, that means when you each ~5ETH in your account), dwarfpool, etc.

**What is a pool?**

Well, imagine an "Ethereum pool" as a normal pool, where you meet with a lot of known or unknown people with an only purpose, have fun. But why just have fun when you can also make some cash together. In an Ethereum pool, "work" is distributed among all users to make the work a lot easier and all the profit is shared with all, based on your personal share.

**Bonus**

So if you want to do a test with your configuration you'll need a video card with at least 2GB memory, preferably an AMD(ATI) video card, but a Nvidia card works too. In the next lines, I will write a beginner tutorial for Windows. First of all, let's download the software that we need to get this job done:

1. The latest drivers for your video cards from the manufacturer from [AMD](http://support.amd.com/en-us/download) or [NVIDIA](http://www.nvidia.com/Download/index.aspx?lang=en-us)
2. An [Ethereum Wallet](https://www.myetherwallet.com/) (from where we will generate a personal wallet address to get the money)
3. The mining software: [Genoil Miner](https://github.com/Genoil/cpp-ethereum/tree/master/releases) - download the latest version and extract to a folder

After we extract the miner to a folder create a batch file that starts our miner, for example, create a new text document and change the extension from .txt to .bat and add this line to it and change according to your wallet:

{% highlight bash linenos %}
  ethminer.exe --farm-recheck 200 -G -S eu1.ethermine.org:4444 -FS us1.ethermine.org:4444 -O 0x04302efb4b3ff14e66c91da0b53decdf3bef0e54
{% endhighlight %}

Save the file and execute it, you'll see something like this:

<img class="img-responsive image-center thumbnail" src="{{site.url}}/img/mining/shell_mining_software.jpg" alt="Started Mining Software" />

Let it work for few hours and check your miner pool status dashboard by accessing this [ethermine.org](http://ethermine.org/) and entering your Ethereum personal address in the white box in the right corner and pressing "Check status" and it will redirect to your statistics.

Hope you enjoyed this and stay tuned for more!