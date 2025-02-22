---
layout: post
title: Convenient and safe intellij LLM plugin
tags: [DevoxxGenie, LLM]
excerpt_separator: <!--more-->

thumbnail: "assets/img/feature-img/devoxxgenie_plugin.png"
---
&emsp; I was looking for some safe (without internet access) LLM model integration which can seamlessly support me with my everyday coding tasks on my mac.
I encountered an interesting looking plugin for IntelliJ - `DevoxxGenie`.<!--more-->

In short, that allows for connecting to a locally running LLM model and using that model to support you in your IntelliJ project.

The easiest way is just to download [ollama](https://ollama.com/download) and the [model](https://ollama.com/search) we would like to use.
This is pretty convenient as we can pick any model that fits (probably simply by testing different models) our needs most.

[//]: # (![img_1.png]&#40;../assets/img/feature-img/ollama_cli.png&#41;)
{% include aligner.html images="feature-img/ollama_cli.png" column=1 %}
{% include aligner.html images="feature-img/devoxxgenie_plugin.png" column=1 %}


Longer description of `DevoxxGenie` by the author: [youtube](https://www.youtube.com/watch?v=kgtctcbA6WE).

&emsp; Everything seems convenient. However, we should put some extra safety here to make sure that it actually won't connect to the internet.
There are 3 potential ways of doing that. I tested 2 of them.

1. Run `ollama` in Docker without network access and connect `DevoxxGenie` to it.
   <br>I have not tested that as there are some issues with this method on Mac.

2. Configure network filters in Mac to not allow `ollama` to connect to the internet (`/etc/pf.conf` file)
   <br>I was able to partially make that work but that is a complicated way to achieve what I want, that is why I tried to find an alternative simpler solution.

3. Use some dedicated application which allows blocking internet connection. I picked [LuLu](https://objective-see.org/products/lulu.html).
   <br>`LuLu` is a free, open-source firewall. Developed by Patrick Wardle, a respected security researcher.

{% include aligner.html images="feature-img/lulu.png" column=1 %}

The best and simplest solution for me is option `3`. Remember to temporarily disable `LuLu` rules when you want to download a new model from `ollama`.

